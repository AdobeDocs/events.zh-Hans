---
title: 从Adobe Analytics迁移到Adobe Customer Journey Analytics的最佳实践
description: 了解从Adobe Analytics迁移到Customer Journey Analytics (CJA)的基本步骤和最佳实践，包括XDM架构设计、数据映射和数据视图设置。
solution: Analytics, Customer Journey Analytics
topic: Migration
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3654
last-substantial-update: 2025-07-16T00:00:00Z
jira: KT-18535
source-git-commit: 90eb4a9d2cf445c58fde776092fb047f820fa207
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# 从Adobe Analytics迁移到Adobe Customer Journey Analytics的最佳实践

了解从Adobe Analytics迁移到Customer Journey Analytics (CJA)。 该研讨会由Adobe Ultimate Success团队的Nicolina Picone和Maurizio Coro主持，深入概述了CJA、其功能以及迁移的最佳实践。

## 讨论的关键主题

* Analytics和CJA之间的差异
* 强身份标识符、调整数据结构和创建可自定义数据视图的重要性
* 涵盖用于导入历史数据、管理营销渠道归因和利用CJA的灵活性进行定制报表的策略

>[!VIDEO](https://video.tv.adobe.com/v/3464911/?learn=on&enablevpops)

## 主要素材

* **Customer Journey Analytics (CJA)概述** CJA是Adobe Analytics的一个发展，侧重于跨多个接触点（例如，移动设备、Web、CRM、呼叫中心）的完整客户历程，而不是单轨事件。 它允许实时数据处理和操作。

* **迁移准备工作**&#x200B;从Adobe Analytics迁移到CJA的关键步骤包括确保强身份标识符（例如人员ID）、对齐变量和维度以及将数据映射到XDM架构。 可通过验证步骤导入历史数据。

* **数据视图和灵活性** CJA允许使用可调整的会话持续时间、分段过滤器和归因设置创建可自定义的数据视图。 这种灵活性允许定制报告和分析。

* **历史数据迁移的最佳实践**&#x200B;通过将CJA数据与可接受范围内（例如，10%差异）的Adobe Analytics数据进行比较来验证该数据。 从较短的回填窗口（例如，一个月）开始，然后逐渐放大。

* **营销渠道归因** CJA为营销渠道归因提供了增强的功能，消除了“访问第一页”功能等限制并启用了更多动态会话配置。
