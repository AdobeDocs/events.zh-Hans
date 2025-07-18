---
title: Adobe Experience Manager as a Cloud Service中的CDN和WAF配置
description: 由Adobe Experience Manager as a Cloud Service专家共享，通过可自定义的CDN规则、WAF保护和配置管道来增强Adobe应用程序的性能和安全性。
solution: Experience Manager as a Cloud Service
feature: Security
topic: Performance, Security
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2211
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16574
exl-id: a9f38e79-c707-443d-8b2f-e534ce4dd43d
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Adobe Experience Manager as a Cloud Service中的CDN和WAF配置

通过可自定义的CDN规则、Adobe保护和配置管道，充分发挥WAF Managed CDN的潜力。 Adobe的高级计算机科学家Marius Petria、Adobe软件开发工程师Quentin Vecchio和Adobe软件开发工程师Florian Froese分享了增强Adobe Experience Manager as a Cloud Service应用程序性能和安全性的策略。

>[!VIDEO](https://video.tv.adobe.com/v/3440612/?learn=on&enablevpops&captions=chi_hans)

## 社区讨论

在Adobe Developers Live社区[讨论](https://adobe.ly/3O0TyYa)中继续对话。

## 要点

* **新配置功能简介**&#x200B;此演示文稿介绍了云服务中CDN的新配置功能，重点介绍为各种用例配置CDN的功能。
* **CDN配置选项**&#x200B;新选项允许与HTTP请求和响应进行交互，例如添加/删除标头、重写请求路径、阻止流量、重定向客户端以及代理到不同的源。
* **安全增强功能**&#x200B;新功能包括流量过滤规则，以根据请求模式阻止或记录流量，以及引入M WAF以针对SQL注入和XSS等Web攻击提供高级保护。
* **声明性配置**&#x200B;配置是使用YAML文件完成的，并通过Cloud Manager中的配置管道进行部署，从而使其成为一个快速而直接的过程。
* **请求和响应转换**&#x200B;新功能允许进行请求转换以标准化URL并删除不必要的查询参数，还允许响应转换以在向客户端发送响应之前设置标头。
* **流量过滤器和速率限制**&#x200B;流量过滤器可以阻止特定的IP或国家/地区，并实施速率限制以防止DDoS攻击。 可根据各种条件（如客户端IP、用户代理和请求路径）配置速率限制。
* **Monitoring and Analysis Tools** Adobe提供了Elasticsearch/Kibana和Splunk功能板等工具，用于分析流量和使用情况，帮助识别和缓解潜在的安全威胁。
* **实践演示**&#x200B;该演示包括演示，演示如何使用Cloud Manager部署CDN配置，以及如何使用AEM在本地处理错误和验证配置。
