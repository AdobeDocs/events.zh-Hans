---
title: 性能交付的最佳实践
description: 利用自适应流、自定义视频配置文件、SEO最佳实践、图像优化、批量内容管理、查看器预设、缓存失效和智能成像，通过Dynamic Media优化媒体交付和性能。
feature: Dynamic Media, Video, SEO Optimization, Smart Imaging, Viewer Presets, Best Practices
topic: Content Management
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1596
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16572
exl-id: a1920020-b9ce-43be-8f9e-e52aac68da7b
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# 性能交付的最佳实践

与Adobe的高级产品经理Riya Midha一起，探索设置Adobe Experience Manager Assets Dynamic Media的最佳实践。 了解如何优化资产交付、增强视频流、配置查看器以及衡量和改进性能。

>[!VIDEO](https://video.tv.adobe.com/v/3440399/?learn=on&enablevpops)

## 社区讨论

在Adobe Developers Live社区[讨论](https://adobe.ly/3YGedpb)中继续对话。

## 主要要点

* **Dynamic Media功能** Dynamic Media支持跨设备快速、灵活地交付高质量、个性化的媒体，每年处理9万亿次以上的媒体交付，每天最高可处理690亿项资产。
* **自适应流**&#x200B;使用自适应流进行视频交付可显着减少缓冲。 一项测试表明，在带宽限制为5 Mbps的情况下，60秒视频的缓冲区数量从50减少到5。
* **视频配置文件**&#x200B;创建具有不同编码质量的自定义视频配置文件可确保在不同网络条件下获得最佳视频性能。
* **SEO最佳实践**
   * 使用规则集创建描述性URL以实现更好的SEO。
   * 向图像添加替换文本和标题属性。
   * 利用智能成像和最新的图像格式（如WebP ）获得更好的搜索排名。
* **图像优化**
   * 使用缩放参数可根据屏幕大小调整图像分辨率。
   * 避免使用100%的图像质量；而应使用80-90%的范围来减小文件大小而不会造成明显的质量损失。
   * 应用锐化参数以增强图像中的文本清晰度。
* **批量内容管理**
   * 将用于Dynamic Media投放的内容与其他内容分离。
   * 使用选择性同步可优化处理时间并缩短上市时间。
* **查看器预设**&#x200B;使用查看器预设自定义查看器外观和行为，无需更改代码。 示例包括编辑播放/暂停按钮、启用自动播放和循环以及添加图像叠加。
* **缓存失效**&#x200B;使用缓存失效立即反映对已发布资源所做的更改，跳过默认的10小时TTL。
* **监视和调试**&#x200B;使用AEM桌面应用程序和查询调试器页面之类的工具来跟踪处理作业并识别未处理的资源。
* **智能成像**&#x200B;默认在所有域上启用智能成像，从而减小图像文件大小并缩短加载时间。
