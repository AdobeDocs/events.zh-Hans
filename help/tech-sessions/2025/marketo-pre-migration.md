---
title: Marketo迁移到Adobe Admin Console — （预迁移）
description: Adobe正在将Marketo Engage迁移到Admin Console，以便更好地管理用户。 了解自动和自助迁移类型、先决条件、迁移后更改、最佳实践、常见隐患以及支持。 访问Adobe Experience League网站上的会议录像。
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2280
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17483
exl-id: 9c3da83f-9e02-4a2e-9784-10213facf056
source-git-commit: 848fa8fee05b315361781059eabb3b19904c78c2
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Marketo迁移到Adobe Admin Console — 预迁移

加入我们，与Adobe专家一起无缝迁移Marketo！

在这个信息性网络研讨会中，借助Adobe的客户体验和身份团队抢先了解Marketo迁移。 我们将向您介绍确保顺利过渡到Adobe Admin Console的关键步骤、最佳实践和常见挑战。

你会学到什么，

* 预迁移流程的分步路线图
* 简化过渡并避免隐患的最佳实践
* 对常见迁移问题的专家解答

无论您是刚刚开始迁移，还是为最终步骤做准备，本课程都将为您提供相关知识和工具，以便您放心地完成迁移过程。 不要错过这个机会，以取得成功并实现您的Marketo无缝迁移！

>[!VIDEO](https://video.tv.adobe.com/v/3449712/?learn=on&enablevpops)

## 主要要点

### 迁移目的和概述

Adobe正在将Marketo Engage迁移到Admin Console，以便将所有产品整合到一个中心位置，从而更好地管理和访问用户。  Admin Console将作为管理Adobe产品、用户角色、权限和支持访问权限的中心中心。 用于访问Marketo Engage的URL将更改为Adobe的Experience Cloud平台。

### 迁移类型

* **自动迁移**&#x200B;适用于用户数少于75且没有SSL设置的组织。 Adobe处理迁移。
* **自迁移**，适用于设置了SSL的组织。 管理员使用迁移控制台管理迁移过程。

### 迁移的先决条件

* 系统管理员必须完成同意电子邮件。
* 必须在Admin Console(而不是Marketo实例)中设置SSL。

### 迁移后更改

* 用户将使用Adobe ID或Federated ID (SSL)登录。
* 管理员角色和权限将决定Admin Console中的访问级别。

### 最佳实践

* 在迁移之前，验证用户电子邮件并解决锁定的帐户。
* 确保分配了适当的管理员角色。
* 禁用广告拦截器或使用无痕模式以避免登录问题。

### 常见陷阱

* 不正确的管理员权限可能会限制访问。
* 浏览器扩展和广告阻止程序可能会干扰访问。
* Admin Console尚不支持将IP列入白名单，但正在开发此功能。

### 对功能的影响

* 自动发送的电子邮件、API用户和Munchkin代码不受迁移的影响。
* 迁移主要影响用户身份验证和管理。

### 支持

* 遇到问题的用户应通过Adobe客户关怀部门发起支持案例。
* 在支持案例中包含IMS组织ID以更快地解决问题。
