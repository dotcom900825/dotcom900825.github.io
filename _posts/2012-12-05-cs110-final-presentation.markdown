---
author: admin
comments: true
date: 2012-12-05 22:56:31+00:00
layout: post
slug: cs110-final-presentation
title: UCSD CS110 Final Presentation后的感想
wordpress_id: 143
---

项目源代码 [ecomstore@github](https://github.com/cs110-2012-fall/ecomstore_12_2-social)
项目进行过程中的所有文档现在仍在修订，学期结束后会放上来

_____________________________

刚刚结束了在ucsd上的cse110 软件工程的 final presentation。 感触很多，想和大家分享一下。

首先介绍一下这门课的形式，Professor  Gary Gillespie 是我们的lecturer， cse110的形式很特殊，Gary实际上以公司的形式来开设这门课程，[]( http://ieng6.ucsd.edu/~cs110f)cs110 fall 2012  Gary是公司的founder和ceo，他手下有两个TA，他们分别是COO，Chief Operating Officer，首席运营官，一个CIO，Chief Information Officer。 还有三四个Tutor，他们是Executive Board Members。专门负责lab时的tutoring。



课程开始时，Gary向我们介绍了这门课的形式，所以学生组队，8~9人的团队，作为公司的一部分，这个学期的主题是电子商务，但没有限定的方案或形式，所以团队可以自己做决定，没有要求实现技术，完全自己决定。

所有组员都有明确的角色分工

Project Manager
Subject Matter Expert: Researches the inner workings of online stores and is involved with how the business rules are integrated into the project.
Senior System Analyst: Coordinator of Use Cases, User Story, Requirements.
Software Architect: Coordinates design, selector of technologies.
Software Development Lead: Coordinates software development.
Algorithm Specialist: Designer of algorithms and module interfaces.
Database Specialist: Maintains database and related issues.
Quality Assurance Lead: Coordinates testing phase, ensures procedures followed.
User Interface Specialist: Focuses on the look and feel, and user experience.                                         每个人根据自己擅长的技术或兴趣选择职位，所有人都会sumbit code，但侧重和工作量不同。

就这样，一周这后，5个小组诞生了。所有的team每周需要参加周一的customer meeting，实际上就是每组展示每周的artifect，来模拟整个软件开发过程，比如User Story，User Case，Database Design etc， 然后Gary逐一点评，每周三还有 Engineer All hand lab，每周都有一个学习主题，比如Version Control使用，html css，mvc design等等。每周各个team还有 team meeting 讨论分工和进行code review，每周每个人要提交time card，来规划每周的时间安排，每两周还有peer review，给自己的组员打分，来评价每个人的贡献，也会给自己打分，得分低的学生与自己给自己打得分和teammate给自己打分差距极大的学生，Gary会单独发邮件沟通。经过三个月的奋斗，终于到了最终presentation的时候。

这门课最后一共有41名学生enroll，分为了5个小组，分别是

Team WIN ——World wide inventory management 我所在的团队，Final Presentation 第二名，一共8个人，我的角色是Software Architect + Software Development Lead 这是我们最后的网站[](http://yuxia.webfactional.com/index.html)Michael Collins Jewelry Store 组长Cory在当地的一家珠宝店兼职工作了很多年，他现在的网站非常旧，[Preview Version](http://www.michaelcollinsjewelry.com/index.php) 而且基本没有server side的支持，完全的静态网页，我们打算为他重新打造一个全新的系统。我们使用的Python Django, Mysql 和Bootstrap + Jquery

Team WTF —— Not what the fuck, is We Trader Fun  8人团队 http://wetradefun.appspot.com/ (没有完全向外界开放)  WTF的点子我非常喜欢，他们决定做一个游戏交换的网站，有点像初中玩GBA那会儿去玉泉东换卡的意思，他们的网站使用了[GiantBomb](http://www.giantbomb.com/) 一个Game Database 网站提供的api来获得所有的游戏信息，你可以搜索所有的游戏信息，然后加入wishlist，然后你可以把你手头闲置的游戏加入到offer list，当有其他人对你的游戏感兴趣他们会给出offer，你则需要从众多offer中选出一个最喜欢的，然后和他交换。 同样使用的Python Django Mysql 和Bootstrap + Jquery


Team OCD —— Over Clocked Developers ， 9人团队 这是他们的最后网站[BuyBox](http://buybox.herokuapp.com/) Final Presentation第一名的团队，他们开发了Buybox网站，类似于一个微型的二手市场，你可以将自己闲置的，想卖的东西发布到上面，感兴趣的买家可以直接给你打款，最大的feature是和社交网络，二维码的结合。 用户发布东西后，可以打印出带有二维码的传单，在学校里散发，当用户扫描二维码后，可以跳转到buybox的网站，而且他们的结账系统非常直接简单，和itunes类似，首先设置后信用卡信息，然后每次决定购买时，一步了当，简单明了，系统非常易于上手，前端的界面也是经过细心雕琢，也适配移动终端。他们下一步打算在UCSD尝试让大家使用，很有可能作为创业的项目。 他们的团队也是强手云集，[Team member](http://buybox.herokuapp.com/ocd)，product manager是HP的工程师，大四学生，一个ruby on rail高手，Quality Assurance Lead是管理科学专业，cs minor，他策划的所有商业方案，并打算明天以他们的网站去做business课程的final presentation。 他们的database specialist 和software architect分别是Carefusion 和 Northrop Grumman的软件实习生，另外一名db specialist是graduate student，ruby高手。两名女生是ui design，每个人都投入了大量的时间和精力在这个项目上，其中一个ui女生和我一开始上cse135课，本来我想和她组队做cs135的项目，但后来她drop了，说要投入精力在她们的网站。 他们使用Ruby on Rails +Mysql + Bootstrap，使用Heroku作为hosting platform



Team WAIT – Wonderful Amazing Inventory Tracking， 他们也有一个真实客户，其中一个组员的妈妈是一个卖眼镜的公司的CIO，他们需要一个Inventory Tracking system来跟踪所有的货物，但因为他们使用的非常过时的数据库，但希望逐步切换到新的技术，于是WAIT team创建了一个Inventory Tracking Website，帮助他们的客户来做这个过渡，功能很强大，可以上传excel表格，并转换格式，呈现在网站上，并能在google map上跟踪所有seller信息，他们的客户非常满意，并打算让他们继续做下去，他们很有可能把系统作为产品，买给这个公司。

用的技术同样是Python Django + Mysql + Bootstrap，Jquery

Team SOL – Software Optimization Logistics 7人团队，做的类似于OCD，也是一个小型的电商系统，但没有很多的创新点，也没有很吸引眼球的feature，[SOL Website](http://sol.csproject.org/) 可以看到他们所有的Artifect，但网站的server [SOL Team](http://sol.csproject.org:8080/) 无法访问。 他们最大的亮点是他们的Artifect，所有的文档都是以网页的形式发布到网上，他们的一个组员是php大牛，写了一个工具来管理这些文档，我是非常佩服。 他们用的技术是Jsp + Mysql + Bootstrap，Jquery



虽然最后大家投票，我们组排名第二，但我自己认为第一当之无愧是OCD，第二是WTF，第三是WAIT，我们排第四，因为论UI，我觉得我们做的一般，网站的功能也非常简单，实现的也是中规中矩的小型电商网站，而WTF有非常好的商业方案和功能实现，如果上线，感觉会发展很快。 WAIT没有绚丽的UI，但很朴实，为它们的客户提供最好的解决方案，专注解决问题。



在ucsd的这个quarter感触最深的就是这门课，和我在北邮上过的课彻底不同，Gary上课基本不怎么讲太细的理论，他在Xerox和SAIC工作了有20多年，是一个Senior Software Engineer，UCSD的本科和研究生，退休后回到UCSD做全职Lecturer，他第一节课就说，I hate teaching Software Engineering, Because you can't learn it unless you actually do it, so I have no idea how to teach at all. 所以真正的课堂就比较奇葩，一般上来他就讲他工作时的一些故事，讲他身边的奇葩工程师，特别二逼的manager，特别照顾他的mentor等等，然后就开始讲Head First Design Pattern，用了三周时间过完了一本书，有用了两周时间过完了Head First Software Development，上课基本没有讲义，直接维基百科，无比飘逸，quiz和midterm都很简单，甚至允许你自己出题，如果题目出的好还给你加分，但真正学东西的是当你做project的时候，和所有队友沟通，交流，分配任务。我的队友Brian，他也是Software Development Lead，一个Chinese，但从来不说中文，开始的两周基本不怎么参与开发，第一次peer review结束后，被Gary单独联系后，开始输出，但往往不能令人十分满意的完成任务，总是给你残缺的东西，然后自己去忙别的，我们的manager cory很负责，他是Cognitive Science的学生，修了Cs的minor，非常喜欢Game Industry，打算以后去暴雪工作做game desiger，Ryan是我们的UI Specialist，非常负责，独自完成了很多design的任务，Josh是Quality Assurance Expert， 这个周末连续工作了两天，测试网站，提出bug，编写测试用例，非常认真，我从一开始就非常认真，投入了很多时间精力在项目上，基本每个周末都在lab里coding，我写了80%的后端系统，和很多前端的页面，我的队友也很信任我，认可我的贡献，两次peer review都给了我满分，对于整个team，最大的问题是能够输出代码的人太少，包括我也是参考着一本Python电子商务实战的书在写，我虽然学过一段时间python，在微软实习的时候也做的web development，但因为对Django不熟，很难完全自己实现一个模块，更何况我的队友了，Steven更偏向硬件，而且手还骨折了，平时所有的文档formatting都交给他，也很难输出，乐哥修了四门课，也没时间精力。好在最后系统成功上线，虽然在交付前有很多bug要调，但毕竟是一个完整的项目，虽然没有OCD的Buybox那么牛逼，但毕竟人家是全员参与，而且很多有经验的developer，我们能拿第二已经很欣慰了。

昨天去听了UCSD在Facebook的实习生的经验交流会，印象最深的就是Facebook不管你的学历和学校或着gpa，他们找的是对互联网有极高热情且聪明的人，有了热情和兴趣，你便愿意投入时间和精力去做某件事，而聪明的人能更快的掌握工具，更短的学习周期和更好的学习效果，加快完成的时间

经过一个学期的项目，有太多的东西要学，html css js还有后端的技术，包括数据库，回国后要静下心来认真学了。下周final week，快回国了！ 争取再找份实习 加油少年！






