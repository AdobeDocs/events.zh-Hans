---
title: 优化AEM性能 — 缓存策略和技术
description: 该会话涵盖了缓存策略和技术、缓存机制和层、动态内容处理、调试缓存问题以及在Dispatcher和CDN之间同步缓存失效。
topic: Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3764
last-substantial-update: 2025-02-21T00:00:00Z
jira: KT-17373
source-git-commit: e7bf8b79ad4920b303fc3afbdfb4adee60614c88
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# 优化AEM性能：缓存策略和技术

在此会话中，我们探究了各种缓存机制（如页面、资产和Dispatcher缓存），以及如何在CDN级别实施缓存以优化内容投放并减少加载时间。 讨论内容将涵盖每个缓存层的最佳实践、常见问题的疑难解答，以及如何利用CDN功能实现最高效率。

## 主要讨论点

* 缓存简介
* 缓存类型、缓存最佳实践、缓存失效和刷新
* 调试技术

>[!VIDEO](https://video.tv.adobe.com/v/3444452/?learn=on&enablevpops)

## 主要要点

* **缓存策略和技术**&#x200B;该会话侧重于用于优化性能的各种缓存策略和技术，包括不同层（如浏览器、CDN和Dispatcher）的缓存。

* **缓存机制和层**&#x200B;讨论涵盖了不同的缓存机制和层，包括浏览器缓存、CDN缓存和Dispatcher缓存，以及如何配置和管理它们。

* **动态内容处理**&#x200B;讨论了用于在页面上处理动态内容的技术，包括使用Sling Dynamic Include (SDI)和Edge Side Include (ESI)，以确保在缓存静态内容时不会缓存动态内容。

* **调试缓存问题**&#x200B;说明了在不同级别（浏览器、CDN、调度程序）调试缓存问题的各种技术，包括使用标头、日志和特定配置来识别和解决缓存问题。

* **缓存失效的同步**&#x200B;会话解决了在Dispatcher和CDN之间同步缓存失效的挑战，建议使用更短的max-age值和CDN清除API以确保在页面激活时两个缓存同时失效。