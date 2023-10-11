---
title: AEM 5.6.1中的作业处理和卸载简介。
description: 获取高级作业处理功能的技术简介。 作业处理是复制和工作流处理等功能的底层基础结构。 了解发现模块以及改进的作业处理API和新功能。
uuid: 181e3781-8eca-4a5d-879e-15ae4e1f6649
discoiquuid: ee4cd526-7363-4b8e-ad26-c2c937b70327
targetaudience: target-audience advanced
exl-id: bd10465b-6f45-4117-b8a0-1310422f5825
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 4%

---

# AEM 5.6.1中的作业处理和卸载简介。 {#introduction-of-job-handling-and-offloading-in-aem}

作业处理是复制和工作流处理等功能的底层基础结构。 这是对高级作业处理功能的技术介绍。 我们将讨论新的发现模块以及改进的作业处理API和新功能。 该卸载框架以作业处理和发现为基础，侧重于在非集群实例之间分发作业。 我们将更详细地了解卸载如何扩展分布式作业处理。 然后，我们查看它如何用于当前的工作流卸载实施，以及如何在自己的项目中使用它。

>[!VIDEO](https://video.tv.adobe.com/v/19580/?quality=9)

*2013年7月24日交付*

**提交人：**

Carsten Ziegeler，Adobe高级开发人员

Marc Pfaff，Adobe首席开发人员

演示者幻灯片 — 第1部分

[获取文件](assets/jobhandling.pdf)

演示者幻灯片 — 第2部分

[获取文件](assets/offloading.pdf)

## 相关链接 {#related-links}

* [Apache Sling事件和作业处理](https://sling.apache.org/documentation/bundles/apache-sling-eventing-and-job-handling.html)
* [Discovery API及其实施](https://sling.apache.org/documentation/bundles/discovery-api-and-impl.html)
* [卸载作业](https://docs.adobe.com/docs/en/cq/current/deploying/offloading.html)
