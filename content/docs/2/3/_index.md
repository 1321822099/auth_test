---
title: "10"
weight: 3
---
![](https://cdn2.ones-ai.cn/images/blog/efficiency-1-8ba6facfee.png)

基于 SAFe 的大规模敏捷协作

![](https://cdn2.ones-ai.cn/images/blog/blog-author-kid-7844741522.png)

冯斌

2019-11-19

随着敏捷开发的普及，各类敏捷管理⽅法已被业界充分实践。但是在数百人或千人级别的研发团队进行协作时，简单的复制小团队的敏捷方法却会遇到诸多问题。

SAFe 作为⽀持⼤型研发团队敏捷落地的一种方式，重新定义了可扩展的敏捷框架模型，同时也降低⼤型团队管理的复杂性。

11月15日，ONES 联合创始人 & CTO 冯斌参加了由 msup 举办的第八届 TOP100 全球软件案例研究峰会，并进行了《大型研发团队敏捷实践落地 - 基于 SAFe 的⼤规模敏捷协作》主题分享，内容聚焦 SAFe 理念下的大规模研发团队管理实践。

案例背景与问题

ONES 项目开始于2016年，专注于企业级研发管理工具。产品研发团队经历了三个发展阶段，每个发展阶段都对应着不同的团队管理方式，以适应产品研发的需求。

初创期：小团队协作——个人物理看板。ONES 的初创阶段，研发团队只有几个人，工作内容相对少，也没有具体的数据需求。这样的情况下使用一个简单的物理看板即可满足团队的管理诉求。

产品 Demo 时期：15人规模团队协作——引入 Scrum。当产品 Demo 完成，团队扩展到了15人左右。像大多数技术型公司一样，在这个阶段 ONES 引入了 Scrum 的模式组成两个小组，两个迭代同时开发，并建立了 CI 等基础设施以完成基本研发流程自动化。在这个过程中是使用 ONES 自身工具来进行 Backlog 和迭代管理的。

成长期：50人规模团队协作——多个 Scrum Team + 矩阵式架构。随着公司业务快速发展，研发团队扩张至50人规模，ONES 的 Scrum Team 增加至6个，兼顾业务效率与职能效率。

但简单复制 Scrum Team 也会有很多弊端：

部门内目标对齐与沟通的问题：局部改进、信息传播效率低

部门间目标对齐与沟通的问题：各部门看问题的角度与价值差异、如何确定全局最优

度量能力缺失的问题：缺少度量手段和方法、如何确定改进方向

团队之间的协作效率会因为更多复杂因素而受到不同类型的制约。ONES 是一家企业服务公司，会有产品部门、销售部门、市场部门等，每个部门在看问题的时候角度不同，就会出现价值上的偏差。

此外，除了各部门间沟通的问题，还会有度量层面的问题，因为项目发展到一定阶段后，需要大量的数据作为支撑来进行产品的优化、性能的改进，如果没有一个度量的手段作为监督，就很难确定这个改进是否达到了真正的效果。

而大型团队的基本管理需求是：

各个敏捷⼩组需要定期的沟通整体业务目标

业务、产品、技术等各类任务需要统⼀制定优先级标准，业务效率优先，兼顾 职能效率

有效的量化方法

面对这些问题和需求，我们需要引入一个更为有效的大规模敏捷方法，因此选择了 SAFe。

ONES 大规模敏捷方案落地过程

SAFe 的一个核心理念，其实可以概括为「分层」。Scrum Team 即团队层，多个 Scrum Team 组成一个项目群（ART），多个项目群组成一个解决方案（SRT），多个解决方案组成一个投资组合（Value Steam）。ONES 主要应用了 Essential SAFe 的部分，在这里讲几个具体实践。

![SAFe大规模敏捷](https://cdn2.ones-ai.cn/images/blog/articles/SAFe-d7f2881112.png)

Essential SAFe

实践一：引入 PI（项目群增量）会议

对于企业服务公司来说，每个月或每季度都会召开需求会议，就是研发、业务等各个部门的负责人一起讨论这一段时间要做哪些需求。PI 会议的性质与其类似。

PI 会议有4类角色：

BO：最终负责人

所有小组 PO（而不是所有人）

SA 小组参加（表达技术改进诉求）

利益相关者也要参加会议（例如销售部门）

在 PI 会议中，我们最主要做的事情是对齐目标和确定各部门全部需求的优先级。对于每一个需求，不同部门都会有一个属于自己的看问题的角度，在这个时候我们可以将这些角度进行处理，最终用优先级去表达。在 SAFe 的框架下有一个 WSJF 的概念去确定优先级。

**WSJF（加权最短作业优先）**

官方维度：WSJF =![](https://cdn2.ones-ai.cn/images/blog/articles/function-9062c4cc8e.png)

ONES 的维度：延迟成本 + 产品/技术价值/故事点

实践二：引入 PI 回顾会议

当我们引入一个计划会议的同时还要引入一个回顾会议，以便总结计划的执行情况。PI 回顾会议类似于敏捷中的迭代回顾，需要演示已完成的功能、收集反馈并将问题加入到 Backlog 中在下一次 PI 会议讨论。

刚刚我们讨论了 Essential SAFe 的两个重要实践，其实在 SAFe 的整体落地中还有两个很重要的方面，分别是「度量」和「DevOps」。

实践三：度量

关于度量，非常重要的一点是一定要使用工具。如果没有工具帮助我们结构化的存储工作数据，我们的工作成果就很难量化，会让工作效率大打折扣。

ONES 使用自身的研发管理工具进行度量以及可视化呈现。我们主要关注端到端的数据，包括客户满意度、特性前置时间、软件发布质量等。

![大规模敏捷可视化](https://cdn2.ones-ai.cn/images/blog/articles/report-514355a16d.png)

项目报表，可视化呈现任务完成情况、代码质量等

实践三：DevOps

DevOps 的概念非常大，我们在这里着重来谈自动化。自动化主要有两点优势，第一点是能够尽早发现问题，降低复杂度；第二点是可以进行更有效的质量内建，创建自动化测试流程，并坚持自动化用例执行率100%才算成功。

总结

在听完 SAFe 的相关理论与实践案例后，大家可能会产生一些疑问，实行 SAFe 到底应该从何处开始？

其实 SAFe 与 Scrum 还有其他敏捷经典理论在本质上是没有冲突的。

SAFe 强调要快速进行流程推进，所以还是需要强调一下工具的重要性。因为工具能够帮助实现流程以及数据的结构化，结构化之后还可以实现将这些数据输出并聚合到数据中台。工具的引入可以固化整个流程，因此项目的推进效率就会随之变高。

![](https://cdn2.ones-ai.cn/images/wechat-qrcode-4272d171b6.png)

相关阅读

[![](https://cdn2.ones-ai.cn/images/blog/blog-header-1-1287f642d2.png)](https://ones.ai/blog-article-header-1.html)

[超级观点](https://ones.ai/blog-article-header-1.html)

[系统化敏捷转型，企业应该这样做](https://ones.ai/blog-article-header-1.html)

[![](https://cdn2.ones-ai.cn/images/blog/blog-author-ones-51921ebbf4.png)](https://ones.ai/blog-article-header-1.html)

[ONES](https://ones.ai/blog-article-header-1.html)

[2020-6-22](https://ones.ai/blog-article-header-1.html)

[![](https://cdn2.ones-ai.cn/images/blog/efficiency-2-59a9b1251c.png)](https://ones.ai/blog-efficiency-2.html)

[高效研发](https://ones.ai/blog-efficiency-2.html)

[敏捷开发与 DevOps 实践原则](https://ones.ai/blog-efficiency-2.html)

[![](https://cdn2.ones-ai.cn/images/blog/blog-author-kid-7844741522.png)](https://ones.ai/blog-efficiency-2.html)

[冯斌](https://ones.ai/blog-efficiency-2.html)

[2018-11-7](https://ones.ai/blog-efficiency-2.html)

[![](https://cdn2.ones-ai.cn/images/blog/efficiency-3-b306a67e0a.png)](https://ones.ai/blog-efficiency-3.html)

[高效研发](https://ones.ai/blog-efficiency-3.html)

[项目总是延期？你需要知道把控项目进展的优秀方法](https://ones.ai/blog-efficiency-3.html)

[![](https://cdn2.ones-ai.cn/images/blog/blog-author-ones-51921ebbf4.png)](https://ones.ai/blog-efficiency-3.html)

[ONES](https://ones.ai/blog-efficiency-3.html)

[2020-6-13](https://ones.ai/blog-efficiency-3.html)

ONES 企业级研发管理工具

更强大的团队协作与项目管理工具，助力企业更好更快发布产品

立即免费试用

产品

[ONES Project](https://ones.ai/project.html)[ONES Plan](https://ones.ai/plan.html)[ONES Pipeline](https://ones.ai/pipeline.html)[ONES TestCase](https://ones.ai/testcase.html)[ONES Wiki](https://ones.ai/wiki.html)[ONES Account](https://ones.ai/account.html)[ONES Desk](https://ones.ai/desk.html)

解决方案

[敏捷研发管理](https://ones.ai/solution.html#scrum)[瀑布研发管理](https://ones.ai/solution.html#waterfall)[DevOps](https://ones.ai/solution.html#devops)

客户案例

[新零售 · 喜茶](https://ones.ai/case-client-xicha.html)[游戏 · 西山居](https://ones.ai/case-client-xishanju.html)[通信 · 中国电信](https://ones.ai/case-client-telecom.html)[人民日报新媒体中心](https://ones.ai/case-client-renming.html)

服务与支持

[产品定价](https://ones.ai/pricing.html)[帮助文档](https://guides-ones.gitbook.io/guides/)[服务团队](https://ones.ai/service-team.html)[ONES Blog](https://ones.ai/blog.html)

关于 ONES

[关于我们](https://ones.ai/about.html)[联系我们](https://ones.ai/contactus.html)[加入我们](https://ones.ai/joinus.html)[合作伙伴招募](https://ones.ai/partners.html)[服务条款](https://ones.ai/service-agreement.html)

下载移动端

![](https://cdn2.ones-ai.cn/images/ones-app-qrcode-094ca99ed6.png)

Copyright ©2020 ONES.AI 深圳复临科技有限公司 [粤ICP备15032127号](http://www.beian.miit.gov.cn/)

![](https://cdn2.ones-ai.cn/images/public-wechat-icon-50b7169a06.png)

关注公众号

![](https://cdn2.ones-ai.cn/images/icon-contact-us-1a7cb132a9.png)

400-188-1518

![](https://cdn2.ones-ai.cn/images/icon-support-email-fa224603fc.png)

support@ones.ai