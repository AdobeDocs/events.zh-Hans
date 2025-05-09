---
title: 为XDM架构建模的最佳实践和见解
description: 在AEP中通过XDM架构、身份管理和最佳实践进行主数据建模，以实现可扩展、实时的个性化和分段。
topic: Personalization
role: Developer
level: Intermediate
doc-type: Event
duration: 3488
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18019
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# 为XDM架构建模的最佳实践和见解

在本课程中，了解创建符合Adobe Experience Platform标准的可扩展、高质量的Adobe Experience Data Models (XDM)的基本最佳实践和快捷方式。 深入了解如何有效地将客户体验和用例数据映射到XDM，以实现跨Adobe和外部工具的无缝集成。

## 讨论点

* 如何定义和组织XDM组件以确保可扩展和灵活的数据模型
* XDM设计、演变和维护中的常见挑战

>[!VIDEO](https://video.tv.adobe.com/v/3458042/?learn=on&enablevpops)

## 主要要点

**Adobe Experience Platform (AEP)中的数据建模**

XDM架构是AEP中数据建模的基础，可实现不同系统之间的数据集成和共享。 它定义了数据的结构和含义，例如用户档案属性和基于事件的操作。

**Identity Management**

正确的身份管理对于避免用户档案崩溃等问题至关重要。 对电子邮件等敏感数据进行哈希处理并使用唯一标识符有助于维护数据完整性。 建议使用身份映射进行实时分段和个性化。

**架构设计最佳实践**

使架构保持简单并专注于营销用例。 避免重载包含不必要属性的架构。 使用标准化的字段组并最大限度地减少可扩展性和面向未来的自定义设置。

**事件与配置文件属性**

决定根据营销目标将数据建模为用户档案属性还是事件。 用户档案属性适用于实时定位，而事件可提供基于时间分段的历史洞察。

**处理折叠的配置文件和可伸缩性**

折叠的配置文件只能由Adobe支持修复，但身份图规则可以防止未来的折叠。 为了重组现有架构，建议提取必要的数据并使用干净的架构重新开始。
