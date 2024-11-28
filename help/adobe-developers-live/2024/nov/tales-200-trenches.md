---
title: 200条战壕的故事
description: 通过优化性能、使用Google PageSpeed Insights、优化LCP和TBT等关键指标、高效管理资源以及遵循开发和图像优化的最佳实践，确保Web项目取得成功。
solution: Experience Manager, Experience Manager Sites
feature: Edge Delivery Services
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1321
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16541
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# 200条战壕的故事

在完成200多个Edge Delivery Services项目后，Adobe高级工程师Kiran Murugulla和Adobe Experience Manager Cloud架构师Varun Mitra分享了所学到的关键经验教训。 探索通过卓越的核心Web动态提供快速、高性能体验背后的秘诀。


>[!VIDEO](https://video.tv.adobe.com/v/3439424/?learn=on&enablevpops)

## 社区讨论

在Adobe Developers Live社区[讨论](https://adobe.ly/4fwWvvi)中继续对话。

## 主要要点

* **性能至关重要**&#x200B;性能，特别是网页的速度，被强调为成功的Web项目的一个关键因素。 首要目标是确保性能得分为100。
* **开发实践**
   * 使用Google PageSpeed Insights在开发期间进行持续测试。
   * 开始使用已获得100分的样板代码的项目以保持高性能。
   * 在合并之前，请确保拉取请求(PR)符合性能标准。
* **关键量度**&#x200B;侧重于优化最大内容绘制(LCP)和总阻止时间(TBT)，因为它们显着影响性能分数。
* **资源管理**
   * 在项目源中包含字体和第三方脚本等必需资源。
   * 使用字体回退可缩短加载时间。
   * 延迟加载非必需脚本以提高初始加载性能。
* **图像优化**&#x200B;优先考虑加载超过优先级的图像，并对关键图像使用高优先级的获取设置。
* **案例研究**
   * ***CNN.com***&#x200B;优化查询索引并延迟加载Google广告以提高性能。
   * ***Herbert Homes***&#x200B;使用交叉观察器API在用户滚动时加载数据，从而提高性能和用户体验。
* **最佳实践**
   * 从样板代码开始，并使用结构良好的标记。
   * 利用高级CSS选择器并最大程度地减少JavaScript操作。
   * 专注于移动优先的开发。
   * 确保内容结构对于作者来说是直观的。
* **工具**&#x200B;使用Google Sheets和DSA等工具来跟踪网站性能分数随时间的变化。

