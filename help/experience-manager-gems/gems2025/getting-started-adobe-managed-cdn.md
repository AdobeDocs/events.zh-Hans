---
title: AEM GEM — 开始使用Adobe托管的CDN
description: 了解如何在AEM Cloud Service中配置Adobe Managed CDN，以通过新的CDN配置功能增强性能和安全性。
role: Developer, User
level: Intermediate
doc-type: Event
duration: 3438
last-substantial-update: 2025-01-30T00:00:00Z
jira: KT-17227
source-git-commit: 1cfa9cdb0e973e6d088b1faeaa63539b0a7fba36
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---


# AEM GEM — 开始使用Adobe托管的CDN

了解AEM Cloud Service中的Adobe托管CDN及其配置方式。 加入我们，探索可用于增强AEM as a Cloud Service应用程序性能和安全性的新CDN配置功能。 在此会话中，您将发现，

* 什么是AdobeCDN
* AEMaaCS和Edge Delivery Services的相关拓扑
* 可以使用CDN规则实施的典型用例
* 如何使用RDE快速测试和部署CDN配置

>[!VIDEO](https://video.tv.adobe.com/v/3443168/?learn=on&enablevpops)

*录制于2025年1月22日*

有问题吗，也许有意见？  加入[Experience League社区](https://adobe.ly/4haufPK)中的讨论！

## 主要要点

### Adobe托管的CDN的主要功能

* **自定义域和证书**&#x200B;托管自定义域和证书以建立安全连接所必需的。
* **缓存**&#x200B;从缓存中传递HTTP响应的速度比从源中提取（数百毫秒）快很多（不到10毫秒）。
* **开箱即用和自定义CDN** Adobe提供了开箱即用的托管CDN，但用户也可以自带CDN。

### 配置选项

* **请求转换**&#x200B;修改标头、重写路径、阻止流量和重定向请求。
* **流量筛选器**&#x200B;根据特定规则阻止或允许流量。
* **身份验证**&#x200B;支持Edge密钥、打孔密钥和基本身份验证。
* **源选择器**&#x200B;根据定义的规则向不同源代理请求。
* **响应转换**&#x200B;修改响应标头和状态。

### 部署和自定义

* **配置管道**&#x200B;部署YAML文件以配置CDN规则。
* **流量保护**&#x200B;使用流量过滤器规则根据模式阻止、记录和警报流量。
* 通过限制每个IP的请求数，针对DDoS攻击&#x200B;**速率限制** Protect。

### 工具和分析

* **ElasticsearchKibana栈栈**&#x200B;使用提供的仪表板分析使用情况和流量。
* **日志转发**&#x200B;将日志转发到Splunk实例以供分析。

### 演示亮点

* **部署配置**&#x200B;演示了部署流量过滤器规则和重定向。
* **身份验证和来源选择**&#x200B;演示了如何设置基本身份验证和到不同来源的代理流量。

### 最佳实践

* **快速响应**&#x200B;确保来自源的快速响应以避免漏洞。
* **良好的缓存**&#x200B;利用缓存高效地处理流量。
* **使用仪表板**&#x200B;分析流量和使用情况以设置适当的速率限制。
* **组合策略**&#x200B;使用不同的速率限制策略以获得更好的保护。
* **设置警报**&#x200B;当网站受到攻击时获取通知。
* **测试规则**&#x200B;在阻止之前开始日志记录操作，以确保规则按预期工作。

### 联系和反馈

* **反馈和用例**&#x200B;联系团队获取高级用例和反馈。
* **未来会话**&#x200B;参与投票以建议未来会话的主题。