---
title: Adobe Experience Manager快速开发环境
description: 如DevOps Life 2024中所述，使用Adobe的新SDK促进云环境中的快速开发和部署，显着缩短部署时间并支持快速更新、实时日志和高级配置选项。
solution: Experience Manager as a Cloud Service, Experience Manager
feature: Developer Tools
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2427
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16570
exl-id: 330d8be1-14a0-488a-aae0-ee90e1f7621e
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Adobe Experience Manager快速开发环境

探索快速开发环境(RDE)和更新的开发人员控制台的最佳实践。 Adobe软件开发工程师Natalia Angulo Herrera和Adobe软件开发工程师Remo Liechti谈到了迁移挑战、AIO CLI设置、部署、测试、日志记录和配置管理，以实现更顺畅的Adobe Experience Manager工作流程。

>[!VIDEO](https://video.tv.adobe.com/v/3440397/?learn=on&enablevpops)


## 社区讨论

在Adobe Developers Live社区[讨论](https://adobe.ly/3UJluDo)中继续对话。

## 主要要点

* **DevOps Life 2024简介**&#x200B;该会话由Adobe的Natalia和Remo主持，侧重于快速开发环境。
* **问题陈述**&#x200B;本地开发环境在本地良好工作但在部署到云时失败的挑战。
* **解决方案**&#x200B;在云中创建新的SDK以促进快速开发和部署，将时间从30分钟减少到几秒或几分钟。
* **部署流程**&#x200B;新环境允许通过新的API和CLI插件进行快速更新和验证，从而加快反馈和部署。
* **基础架构差异**&#x200B;云环境使用单个创作和发布实例，没有高可用性，并且不使用MongoDB。
* **设置和使用情况**&#x200B;开发人员可以通过云界面设置快速开发环境，使用npm和Adobe IO CLI进行安装和配置。
* **基本命令**&#x200B;关键命令包括io amd —help、io登录、io状态、io安装、io历史记录、io删除和io重置。
* **日志记录和调试**&#x200B;新环境支持实时日志和更改日志级别，无需重新部署，使用io am或d logs之类的命令。
* **高级主题**&#x200B;支持前端包和配置管道，允许快速部署和迭代。
* **即将推出的功能**&#x200B;计划引入快照功能，以便更轻松地重置环境和自动更新，而不会丢失内容。
* **问答和反馈**&#x200B;此会话鼓励参与者加入Discord渠道以便与开发团队进行实时交互和反馈。
