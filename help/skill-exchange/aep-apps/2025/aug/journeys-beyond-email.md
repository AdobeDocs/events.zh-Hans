---
title: 解决电子邮件以外的Adobe历程
description: 了解如何使用Adobe Journey Optimizer设计和测试多渠道历程，使用测试用户档案、事件数据和现实情景实现最佳参与。
feature: Email, Direct Mail, Journeys
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-08-28T00:00:00Z
jira: KT-18850
source-git-commit: a633bfda2c2067c6eb34a8743665993dbceea660
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# 解决电子邮件以外的Adobe历程

本会议通过一个具体的示例探讨了如何解决Adobe Journey Optimizer中的实际挑战。 它重点介绍了跨电子邮件、语音和直邮构建多接触点历程的策略，以创建一致的客户体验。 与会者将从产品所有者的角度获得切实可行的见解和方法以优化历程。

## 关键要点

* 使用特定的跨渠道历程映射分解现实世界中的问题。
* 每个问题都存在多个有效的解决方案 — 灵活性是关键。

>[!VIDEO](https://video.tv.adobe.com/v/3471331/?learn=on&enablevpops)

## 应用实际历程场景

* **定期付款拒绝**&#x200B;当捐赠者的每月付款失败时，触发多渠道响应以解决问题并维护关系。
* **渠道选择**&#x200B;首先使用电子邮件，如果电子邮件退回或未执行操作，则使用直邮或致电。
* **Personalization**&#x200B;根据捐赠者数据（如子赞助详细信息）调整邮件以使通信相关。
* **可扩展性**&#x200B;设计历程以最大限度地减少团队参与并简化未来的更新。

## 逐步设计多通道历程

* **识别事件**&#x200B;通过识别定期信用卡拒绝开始。 这将触发历程。
* **将数据发送到AEP**，将拒绝事件批处理到Adobe Experience Platform中的自定义数据集。
* **划分历程**&#x200B;创建三个微历程 — 电子邮件通知、直邮和出站呼叫。 每个报表使用不同的数据和计时。
* **个性化通信**&#x200B;使用电子邮件事件数据、打印和呼叫的配置文件数据。 提前规划，以便每个渠道都有正确的数据可用。
* **监控响应**&#x200B;根据客户操作（如电子邮件打开、点击或付款解析）调整历程以确定后续步骤。