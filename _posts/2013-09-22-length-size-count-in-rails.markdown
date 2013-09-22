---
author: admin
comments: true
date: 2013-09-22 15:39:00+00:00
layout: post
slug: count-length-size-rails
title: length, size, count, in Rails 3.2.3
category: tech
tags: Rails ActiveRecord
---

Before the new semester begins, I read a lot of Rails best practices, one book is really helpful:  **[Rails Antipattern](http://www.amazon.com/Rails-AntiPatterns-Refactoring-Addison-Wesley-Professional/dp/0321604814)**.  I read about a little trick that reminds me of the days working in Fishtrip.cn.

When I was developing the order statistic product, I need to count the number of total orders. So I do this: ``Order.succeed.all.length``.  However, on the code review, our tech lead Medal Huang told me that this would result in bad performence and I should use count or size instead. I was not sure about the difference between those three method calls. And until now when I was reading Rails Antipattern, in chapter 8 Scaling and Deploying there is a comparison between those three methods and explanation.

* @article.comments.count
* @article.comments.length
* @article.comments.size

**length** will load all your objects just to count them; something like:

    select * from comments...
and then return the results count.
As you can imagine - it's gonna be slow and inefficient.

**count** will just issue

    select count(*) from comments...
which is better, because we are not loading all comments just to count them

**size** is smarter - it'll check if the association is already loaded and if true then return the length (without issuing a call to the database).

source:

	def size
     loaded? ? @records.length : count
	end

**size** also checks for **counter_cache** if you have a field named **comment_count** in your article model, then size will use this field for the count, so there is no need to issue a count on the comments table.

if all fails, **size** will issue a `select count(*)` on the database
