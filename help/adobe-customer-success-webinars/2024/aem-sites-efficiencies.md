---
title: AEM Sites效率 — 性能优化、配置和故障排除
description: 关于AMP站点效率的网络研讨会涵盖了性能优化、Dispatcher配置、权限管理最佳实践以及解决性能问题的策略。
solution: Experience Manager
version: Experience Manager as a Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
exl-id: 55f7c1d8-7c2c-4392-894a-2aa9b3cc0e4a
source-git-commit: 5c946ab73e78d4243ca310032a10bb8e82228c3d
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# AEM Sites效率：性能优化、配置和故障排除

在本网络研讨会中，我们将深入探讨Adobe Experience Manager (AEM) Sites故障排除的要点。 无论您是面临性能问题还是处理复杂的配置，本课程都将为您提供维护和优化AEM环境的实用技能。 我们将优先使用实时演示而不是幻灯片，在应对现实世界挑战方面提供实践经验&#x200B;。

>[!VIDEO](https://video.tv.adobe.com/v/3435114/?learn=on)

## 要点

此网络研讨会重点介绍AMP站点效率，包括性能优化、配置和故障排除。

### Dispatcher配置

* Dispatcher在提供高性能网站方面的重要性。
* Dispatcher配置的关键方面：虚拟主机配置、具有缓存结构的域映射以及定期报告和重定向。

### Rights Management

* 最佳实践：将权限应用于组、避免拒绝报表和避免过度工程。
* 使用Netcentric ACL工具通过Yaml文件管理权限，确保易于部署和跟踪。

### 性能问题

* 在同步操作中标识增量以避免完全缓存刷新的重要性。
* 避免在工作时间执行大型页面操作。
* 将工作流简化为必要的步骤。
* 在创作系统上处理第三方系统流程时请务必谨慎，尤其是使用ImageMagick等工具时。
* 避免向无法处理该加载的第三方系统发送同步请求。
* 管理繁重的自定义组件以避免性能下降。
* 监视长时间运行的会话，以防止出现未找到区段的异常。
