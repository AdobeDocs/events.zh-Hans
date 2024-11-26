---
title: 使用Web组件滚动您自己的HTML
description: 与Raymond Camden， Sr. Developer Evangelist一起学习Web组件基础知识，Adobe包括自定义元素、影子DOM和HTML模板，以及嵌入PDF和构建可排序表等实际示例来增强您的应用程序。
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2580
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16579
source-git-commit: 8770c8172ee90524079efc65aec7e129f1d1d031
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# 使用Web组件滚动您自己的HTML

与Adobe的资深开发人员宣传专员Raymond Camden一起学习Web组件基础知识，包括自定义元素、影子DOM和HTML模板。 探索嵌入PDF和构建可排序表等实际示例，以使用可重用的现代解决方案增强您的应用程序。

>[!VIDEO](https://video.tv.adobe.com/v/3440406/?learn=on&enablevpops)

## 社区讨论

在Adobe Developers Live社区[讨论](https://adobe.ly/48PRE63)中继续对话。

## 关键要点

* **Web组件简介** Web组件允许开发人员创建具有自己的外观和交互性的自定义HTML元素，并使用JavaScript进行定义。
* **Core Technologies** Web组件是使用三种核心技术构建的：自定义元素**影子DOM和HTML模板。
* **自定义元素**&#x200B;自定义元素允许创建新的HTML标签。 它们必须使用烤肉串大小写并包含短划线。 JavaScript类用于定义其行为。
* **影子DOM**&#x200B;影子DOM为组件的DOM树提供封装，防止CSS泄露并允许更可控的样式。
* **HTML模板** HTML模板允许定义可以克隆并附加到DOM的HTML和CSS。 但是，演示者更喜欢使用版块而不是模板，以获得更好的分发和灵活性。
* **属性和事件**&#x200B;自定义元素可以具有属性和事件处理程序（如connectedCallback和disconnectedCallback），以便在从DOM中添加或删除时管理其行为。
* **插槽**&#x200B;允许将内容插入到Web组件中，同时支持默认插槽和命名插槽，以实现更灵活的内容管理。
* **真实示例**&#x200B;示例包括PDF嵌入查看器、图像占位符和表排序器，用于演示Web组件的实际应用。
* 如果JavaScript加载失败，**渐进式增强功能** Web组件可以增强现有HTML而不中断功能。
* **后续步骤和资源**&#x200B;演示建议探索表单参与率、声明性影子DOM、自定义HTML属性和服务器端渲染。 资源包括MDN、webcomponents.org以及Ben Farrell撰写的“Web组件正在运行”一书。