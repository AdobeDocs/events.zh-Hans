---
title: Assets迁移蓝图
description: 了解如何利用Achim Koch提供的见解将旧版DAM迁移到Adobe Experience Manager Assets，其中涵盖利益相关者分析、资源规划、数据转换和最佳实践，例如使用CSV文件进行数据处理。
feature: Migration
topic: Migration
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1690
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16576
exl-id: f588055b-05c7-44df-be67-799a0e3ee1ed
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Assets迁移蓝图

与Adobe的首席技术架构师Achim Koch一起了解如何将旧版DAM迁移到Adobe Experience Manager Assets。 深入了解利益相关者分析、资源规划、数据转换和最佳实践，例如使用CSV文件进行数据处理。 为您自己的Adobe Experience Manager迁移项目构建路线图。

>[!VIDEO](https://video.tv.adobe.com/v/3440403/?learn=on&enablevpops)

## 社区讨论

在Adobe Developers Live社区[讨论](https://adobe.ly/4hKHpnF)中继续对话。

## 主要要点

* **没有现成的迁移工具**&#x200B;由于产品和自定义解决方案的多样性，没有单一工具可以从各种旧版系统迁移到Adobe Experience Manager (AEM)。

* **迁移的五个阶段**

   * 项目计划
   * 实施规划
   * AEM实施
   * 迁移脚本实施
   * 迁移执行

* **利益相关者参与**&#x200B;确定利益相关者（如发起人、商业用户、IT系统管理员和旧版系统支持）并让其参与至关重要。

* **资源和时间线规划**&#x200B;确保资源可用，并围绕假日、高峰期和超限窗口进行规划。

* **技术规划**&#x200B;这包括需求分析、数据转换和基础架构规划。

* **迭代进程**&#x200B;迁移涉及脚本执行、分析、反馈和适应的多次迭代。

* **首选使用CSV文件** CSV文件，以便在迁移过程中易于使用和阅读。

* 推荐使用&#x200B;**脚本语言** Node.js，因为它支持CSV、AWS和HTTP，并且是学习JavaScript的好机会。

* **质量和重复性**&#x200B;确保高质量的数据迁移，保留原始数据和CSV文件以供参考，并使过程可重复。

* **内容冻结**&#x200B;在迁移期间声明内容冻结，以防止在拍摄快照后添加新数据。

* **工具和提示**&#x200B;使用VS代码等工具和Rainbow CSV扩展名，并考虑UTF-8文本文件的字节顺序标记(BOM)。

* **业务批准**&#x200B;保留在迁移后测试和获取正式业务批准以解除内容冻结的时间。
