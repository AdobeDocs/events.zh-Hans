---
title: 优化内容交付 — 释放Edge服务的强大功能
description: 关于Edge Delivery Services (EDS)的座谈会介绍了其体系结构、与基于文档和基于AEM的创作的集成、快速站点创建、自定义选项以及保持高性能的最佳实践。
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
topic: Headless, Integrations, Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
exl-id: 2057e491-9ec3-4bfe-b85a-6b74d70822bf
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# 优化内容投放：释放Edge服务的强大功能

在此会议中，我们将概述Edge Delivery Services (EDS)及其架构。 我们将探讨EDS如何通过通用编辑器与基于文档的创作和基于AEM的创作集成。 一个实时演示将展示EDS的实际操作情况，然后是进一步的探索和问答资源。

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## 关键要点

### EDS简介

* EDS是一组可组合服务，旨在增强ATM的功能。  
* 它旨在提供卓越的体验，通过快速的开发周期和100%的灯塔分数促进参与和转化。  

### 创作选项

* **基于文档的创作**&#x200B;使用熟悉的工具（如Microsoft Word或Google Docs）创建内容，无需进行大量培训即可快速创建内容。  
* **通用编辑器**&#x200B;提供了类似于传统ATM站点的WYSIWYG界面，允许创建更详细和可视化的内容。  

### 架构

* EDS集成在Amazon Cloud Service框架中。  
* 它支持无服务器实施，并且可以在没有传统作者或发布者实例的情况下工作。  
* 可以实施两个级别的缓存：在客户基础架构级别和EDS级别。  

### 内容管理

* 基于文档的创作需要GitHub帐户、Google Drive或Microsoft SharePoint、Sidekick插件和代码同步工具。  
* 具有IAM创作功能的EDS需要GitHub帐户、IAM as a Cloud Service许可证和代码同步工具。

### 开发和部署

* 使用EDS创建站点的过程非常快，通常只需不到一天即可完成。  
* 可以使用aem up命令进行本地开发，以创建网站的本地版本。
* 更改可以提交到功能分支以供测试，然后再合并到主分支。  

### 自定义和可扩展性

* 可以使用简单的CSS和JavaScript创建自定义组件。  
* 该架构允许第三方集成和自定义创作源。

### 最佳实践

* 推荐使用vanilla JavaScript和CSS来保持较高的Lighthouse分数。
* 应仔细考虑和测试任何引入的库（如React），以避免性能下降。

### 支持和文档

* 提供了全面的文档，以指导用户完成设置和自定义过程。  
* 对于任何未解决的问题，鼓励用户联系Adobe支持团队。  
