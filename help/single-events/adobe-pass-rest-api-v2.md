---
title: Adobe Pass — 新的REST API v2
description: 此会议重点介绍Adobe的新REST API v2以及指导用户完成其迁移过程。
role: Developer
solution: Pass
level: Beginner, Intermediate, Experienced
doc-type: Technical Video
duration: 3230
last-substantial-update: 2025-04-07T00:00:00Z
jira: KT-17685
hidefromtoc: true
exl-id: 745411bb-48d7-4410-a236-d02c2927ac1b
source-git-commit: 088615f28aa91dfd4ba119c11c4c9f8a89441d84
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Adobe Pass — 新的REST API v2

此会议重点介绍Adobe的新REST API v2以及指导用户完成其迁移过程。

>[!VIDEO](https://video.tv.adobe.com/v/3457461/?learn=on&enablevpops)

## 主要亮点

* **概述和优点**

   * REST API v2专为现代、灵活和可扩展的身份验证而设计，可满足高需求事件和多设备场景。
   * 密钥改进包括增强的加密、会话一致性、跨设备SSO和扩展的错误信息以加快调试。

* **迁移步骤**

   * 用户必须创建新的注册应用程序，这些应用程序具有REST API v2作用域。
   * 可以重用设备识别和MVPD映射等现有配置。
   * 迁移涉及注册、配置、身份验证、预授权和授权等阶段。

* **功能增强**

   * 统一的RESTful API取代了访问邻居SDK，从而简化了跨平台的实施。
   * 支持在同一会话中使用多个身份验证配置文件以及无缝的跨设备过渡。
   * 对于内容访问，预授权和授权流程仍然是必需的。

* **时间线**

   * REST API v1将在2025年12月停止接收更新，并在2026年底完全停用。
   * 我们鼓励用户早在这些截止日期之前完成迁移。

* **资源和支持**

   * Adobe Experience League上提供了文档、指南和常见问题解答。
   * Adobe提供沙盒环境、Zendesk票证和迁移会议以寻求支持。

* **问答要点**

   * REST API v2需要重新身份验证，因为它与v1无法向后兼容。
   * 预授权用于UI目的，而媒体令牌需要授权。
   * 通过新的Adobe服务令牌支持SSO。
