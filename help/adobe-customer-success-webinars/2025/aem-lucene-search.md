---
title: AEM Lucene搜索的基本提示和最佳实践
description: 使用高级的AEM搜索工具（如过滤器、Facet、自动建议、NGram和拼写检查）提升数字参与度。 从实际演示中学习。
solution: Experience Manager
feature: Search
role: Admin, Developer
level: Intermediate, Experienced
doc-type: Event
duration: 3630
last-substantial-update: 2025-11-13T00:00:00Z
jira: KT-19550
source-git-commit: 84c9a126769fa94b0197d12ca594137e13edc510
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# AEM Lucene搜索的基本提示和最佳实践

了解如何使用前沿搜索功能（包括过滤器、Facet、自动建议、NGram和拼写检查）增强您的数字形象并提高客户参与度。 从实际演示中学习，并深入了解如何使用AEM和Lucene优化您的搜索功能。 此网络研讨会为您提供提升搜索体验并在数字环境中保持领先地位的机会。

>[!VIDEO](https://video.tv.adobe.com/v/3476410/?learn=on&enablevpops)

## 解锁Adobe Experience Manager中的强大搜索

Adobe Experience Manager (AEM)利用Lucene搜索跨内容、资源和元数据提供快速的相关结果。 本课程探讨Lucene索引的工作原理、配置方法以及最大化搜索性能的最佳实践。

* **Lucene搜索无处不在**&#x200B;支持AEM创作、发布者和门户中的搜索，处理自动建议、筛选器、Facet和分页。
* **索引定义驱动性能**&#x200B;自定义Oak索引定义对于高效的目标搜索至关重要。
* **最佳实践问题**&#x200B;复制现有的索引定义，限制索引属性，并使用正确的标志进行全文和属性搜索。
* **高级功能增强UX** Facet、自动建议、拼写检查、提升和词干处理可以为更丰富的搜索体验启用。

了解这些原则有助于确保AEM中稳定、高价值的搜索功能，同时支持技术和业务目标。

## Lucene索引构建基块

AEM Lucene索引定义是搜索性能和准确性的基础。 关键组件包括：

* **Type**&#x200B;指定索引类型（Lucene、属性等）。
* **节点类型限制**&#x200B;针对特定内容类型（例如，dam:Asset、cq:Page）。
* **路径限制**&#x200B;为了提高效率，将索引限制为定义的存储库路径。
* **聚合规则**&#x200B;控制索引内容的深度和范围，确保相关属性可搜索。
* **索引规则**&#x200B;核心配置；设置nodeScopeIndex（广泛全文搜索）等标志和已分析标志（标记化/标准化）。

仔细配置这些元素可确保搜索查询快速、相关且资源高效。

## 优化搜索性能

AEM Lucene中的有效搜索优化涉及战略配置和遵循最佳实践：

* **从现有索引开始**&#x200B;始终复制和修改开箱即用的定义，从不从头开始构建。
* **限制索引属性**&#x200B;仅包含使索引保持精简和性能所需的属性。
* **明智地使用标志：
   * **nodeScopeIndex** true用于广泛全文搜索
   * **已分析** true，属性级标记化
   * 基于路径的查询&#x200B;**evaluatePathRestriction** true
* **属性索引**&#x200B;首选属性限制搜索以获得最佳性能；仅在需要时使用全文。
* **排序和Facet**&#x200B;启用propertyIndex和排序顺序；将facet设置**true可基于计数进行筛选。

应用这些策略可加快查询、减少资源使用并产生更相关的结果。

