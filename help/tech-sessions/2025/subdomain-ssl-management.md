---
title: 技术研讨会 — Adobe Campaign子域和控制面板中的SSL管理
description: 了解如何在Adobe Campaign控制面板中委派和配置子域、设置SSL证书以及监控配置以确保安全电子邮件可投放性。
solution: Campaign
feature: Subdomains and Certificates
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3409
last-substantial-update: 2025-09-05T00:00:00Z
jira: KT-18866
source-git-commit: 18ce421793d97372198151afc92b24f3bed053a8
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# 技术讲座：控制面板中的Adobe Campaign子域和SSL管理

在此会话中，我们探究了Adobe Campaign中子域委派和配置的概念，包括安装SSL证书以保护子域。

了解子域是什么、其用途以及使Adobe能够有效地使用它的委派方法。 该课程还介绍了通过SSL证书保护子域的原则以及维护安全环境的最佳实践。

我们提供了有关使用自助控制面板配置子域的分步指南，其中重点说明了潜在障碍以及如何解决这些障碍。 参与者将获得实用的知识，以确保顺利设置子域并对子域进行安全管理。

无论您是管理员、开发人员还是平台所有者，此会话都能让您掌握在Adobe Campaign中自信配置和保护子域的技能。

>[!VIDEO](https://video.tv.adobe.com/v/3471391/?learn=on&enablevpops)

## 掌握Adobe Campaign中的子域管理

解锁Adobe Campaign电子邮件通信的子域委派、配置和安全的要点：

* **子域委派**&#x200B;选择完全委派或CNAME委派，以控制Adobe如何管理您的DNS和电子邮件投放能力。
* **DNS和SSL设置** MX、SPF、DKIM、DMARC和SSL证书的正确配置对于安全、可靠的电子邮件发送至关重要。
* **控制面板**&#x200B;使用Adobe的自助服务工具简化子域设置、监视记录和管理SSL证书。
* **常见隐患**&#x200B;通过了解审核时间表、记录要求和故障排除步骤，避免延迟和错误。

掌握这些流程可确保您的营销活动安全、可交付，并维护您的品牌声誉。

## 委派方法**完整与CNAME

* **完全委派** Adobe管理子域的所有DNS记录，确保最佳可投放性和安全性。 为大多数用户推荐。
* **CNAME委派**&#x200B;客户和Adobe共享DNS职责。 客户创建指向Adobe管理的资源的CNAME记录。
* **主要区别：
* **Full** Adobe拥有完全权限；客户维护较少。
* **CNAME**&#x200B;分担责任；为客户提供更多手动步骤。
* **提示**&#x200B;永远不要委派根域（仅限子域），以免失去对主域的控制。
