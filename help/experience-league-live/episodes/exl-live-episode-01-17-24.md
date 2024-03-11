---
title: 将Adobe Analytics数据和分析导入Customer Journey Analytics
description: 了解新的自动化流程如何帮助您将分析和数据从Adobe Analytics移动到Adobe Customer Journey Analytics。
jira: KT-14746
thumbnail: https://video.tv.adobe.com/v/3426778?format=jpeg
event-cta-url-live: https://www.youtube.com/watch?v=BkAjaMPgpgE
event-cta-url-reg: https://engage.adobe.com/ExpLeagueLive-240117.html
event-start-time: 2024-01-17 10:00-7
event-guests: Doug Moore,Eric Matisoff,Bryan Skelton
exl-id: 2c2136a9-0b40-4a0a-907d-5af181568073
duration: 3655
source-git-commit: 604f85ddc402ed248678782412efe4f2e5988ab4
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 将Adobe Analytics数据和分析导入Customer Journey Analytics

与Bryan、Eric和Doug一起讨论如何快速开始使用Customer Journey Analytics(CJA)。 您将了解如何使用自动化流程将数据和分析从Adobe Analytics移动到CJA，以及流程中要考虑的任何问题。 当然，他们在此过程中还会有不少有趣的技巧和窍门。

>[!VIDEO](https://video.tv.adobe.com/v/3426778/?quality=12&learn=on)

>[!BEGINSHADEBOX “有疑问吗？”]

继续讨论 [Experience League社区论坛讨论](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/experience-league-live-post-session-discussion-bringing-your/m-p/646093#M3582).

>[!ENDSHADEBOX]

## 要点

* 可通过两种方式将数据从Adobe Analytics导入Customer Journey Analytics：Analytics Data Connector (ADC)和Web SDK。
* ADC允许将报表包中的数据复制到Adobe Experience Platform中进行分析，而Web SDK将数据直接发送到Adobe Experience Platform中。
* Customer Journey Analytics中的数据视图提供了一种自定义和分析引入平台的数据的方法。
* 数据视图提供了强大的功能，例如追溯性更改、用于自定义的派生字段以及在粒度级别过滤和分析数据的能力。
* Customer Journey Analytics中的连接允许合并不同的数据集，从而允许在一个位置分析多个数据源。
* 应战略而谨慎地使用数据视图和连接，以确保对数据访问和分析进行适当的治理和控制。
* 新增了一个名为“组件迁移”的工具，它允许Adobe Analytics管理员将项目迁移到CGA。
* 在迁移项目时，表中的所有组件以及应用的任何区段或计算量度都会移至CGA。
* 存在一个映射过程，在此过程中，可以使用catch-all或派生字段来映射CGA中不存在的组件。
* 建议为CGA中不存在的元素创建一个全包项，然后在目标项目中编辑它们。
* 以前，人们认为在迁移到CGA时必须重新创建计算量度和区段，但现在有一种方法可用来迁移它们。
* 要确保在迁移中包含计算量度和区段，需要将这些量度和区段应用于Adobe Analytics中的表或可视化图表。
