---
title: 使用Cloud Manager简化DevOps
description: 使用Adobe在AMP Cloud Manager中新增的“自带Git”功能优化部署工作流，允许直接集成外部Git存储库，支持用于早期代码质量检查的左移策略，并提高效率和适应性。
solution: Experience Manager, Experience Manager Cloud Manager
feature: Git Repositories, CI-CD Pipeline
topic: Integrations
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1034
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16547
source-git-commit: a5b6c2c3150fcc98686fe74d68f186bfe4e1befa
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---


# 使用Cloud Manager简化DevOps

高效的DevOps实践对于大规模交付体验至关重要。 Adobe软件开发工程师Adrian Tanase探讨了Adobe Experience Manager Cloud Manager如何简化部署工作流、增强自动化并支持持续集成和交付(CI/CD)。

>[!VIDEO](https://video.tv.adobe.com/v/3439904/?learn=on&enablevpops)

## 社区讨论

在Adobe Developers Live社区[讨论](https://adobe.ly/3Ywf7Vm)中继续对话。

## 主要要点

* **新功能简介** Adobe的Adriana Clayton在AMP Cloud Manager中引入了名为“自带Git”的新功能。
* **该功能的用途**&#x200B;该功能旨在优化部署工作流，使其更快、更高效并适应首选供应商。
* **已解决挑战**&#x200B;该功能解决了将外部Git存储库与AdobeGit存储库同步的复杂性，这给部署过程增加了额外的步骤和时间。
* **提供的解决方案**“自带Git”允许将专用和公共外部Git存储库直接连接到Cloud Manager管道，从而能够在代码合并之前即时感知代码更改并运行操作。
* **向左切换策略**&#x200B;集成支持向左切换策略，允许在开发过程中更早运行代码质量检查，从而及时向开发人员提供反馈。
* **演示和验证**&#x200B;提供了一个演示，其中演示了如何使用Cloud Manager集成和验证存储库，包括GitHub和Bitbucket存储库的步骤。
* **客户影响**&#x200B;自其正式发布以来，已有130多个客户登录了其存储库，阻止了2500多个存在代码质量问题的拉取请求进入生产环境。
* **未来增强功能**&#x200B;计划扩展该功能以直接在GitLab和Bitbucket中包含报告，并将“自带Git”扩展到Edge交付服务，以获得更大的灵活性。
* **鼓励反馈**&#x200B;鼓励客户提出反馈并参与非GitHub存储库的早期采用者阶段。
