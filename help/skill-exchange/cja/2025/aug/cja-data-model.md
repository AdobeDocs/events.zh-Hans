---
title: 分析的架构 — 如何处理Customer Journey Analytics数据模型
description: 了解如何使用事件层级、归因和KPI来构建CJA数据模型，以解锁更深入的客户历程洞察。
feature: Attribution
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-09-04T00:00:00Z
jira: KT-18813
source-git-commit: 124b52203b98a80dd9202dab1b0dbe575475a52b
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 分析的架构：如何处理Customer Journey Analytics数据模型

构建CJA数据模型的一个关键方面是了解不同接触点和交互之间的层次关系。 这为进行有意义的分析和洞察奠定了基础。

主要考虑因素包括：

* 识别并映射所有渠道的客户互动点
* 建立明确的事件层次结构和关系
* 定义一致的归因模型
* 创建标准化量度和KPI

通过正确构建这些元素，组织可以更好地跟踪和分析完整的客户历程，从而获得更切实可行的见解并改进决策能力。

>[!VIDEO](https://video.tv.adobe.com/v/3471111/?learn=on&enablevpops)

## 为强大的Analytics解锁数据建模

了解Adobe Experience Platform (AEP)和Customer Journey Analytics (CJA)中的有效数据架构如何推动切实可行的洞察和报表。

* **架构设计很重要**&#x200B;平面架构、阵列和对象阵列之间的选择将直接影响分析能力和报告灵活性。
* **转换流程**&#x200B;摄取到AEP中的数据必须经过周密的结构化，以确保在CJA中进行无缝转换和使用。
* **容器层次结构**&#x200B;了解事件、会话和人员级别对于多级别分析和准确报告至关重要。
* **实用策略**&#x200B;前期规划、架构治理和利用平台功能是可扩展的、面向未来的实施的关键。

掌握这些概念可使团队优化其分析工作流并解锁更深入的业务洞察。

## 架构类型及其用例

* **平面架构**&#x200B;最适合直接的一对一数据关系。 非常适用于基本事件跟踪和简单的量度/维度。
* **数组**&#x200B;对于相关项目（如产品类别、内容标记）的列表很有用。 每个数组元素都成为用于分析的单个维度。
* **对象数组**&#x200B;专为产品购买等复杂用例而设计，其中每个对象都维护其自己的属性和关系。 启用详细的对象级别分析。
* **明智选择**&#x200B;选择最简单的架构以满足您的需求，但针对需要保留关系的高级方案利用数组和对象。