---
title: 咨询专家 — 标记中的有用扩展(Launch)，帮助对Web SDK充值
description: 您是否考虑将实施迁移到新的AdobeWeb SDK？  我们将在Adobe标记库中运行一些我们喜爱的扩展，这些扩展可帮助您将数据收集提升到新的水平。
solution: Data Collection,Experience Platform
kt: 10528
thumbnail: https://video.tv.adobe.com/v/346610?format=jpeg
event-start-time: 2022-08-23 09:00-7
event-cta-url: null
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
source-git-commit: 3d2289642f4164bf82dc1c8a42c5798e9183188b
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# 询问专家：Tags (Launch)中的有用扩展，可帮助对Web SDK充值

您是否考虑将实施迁移到新的AdobeWeb SDK？  我们将在Adobe标记库中运行一些我们喜爱的扩展，这些扩展可帮助您将数据收集提升到新的水平。

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## 节目中的问题和评论

### Evolytics中的数据元素助手扩展

<br> 
**问题：** 从数据安全的角度来看，使用Evolytics是否安全，因为这是第三方扩展？

**回答：** 是。 您可以根据需要查看扩展代码，它不会保存任何日期，只是执行转换。

<br> 

**问题：** 这是否也会捕获AdobeECID？

**回答：** 该扩展中未捕获AdobeECID。 此扩展用于创建额外的匿名标识符（以及其他内容）。

**回答：** 但是，可以通过其他方式捕获AdobeECID。 我们将通过ExL笔记和Twitter分享这些信息，因为我们无法在此聊天中分享链接。

<br> 

**问题：** 哈希功能是否提供各种哈希技术（如SHA-256）并提供公钥和私钥？

**回答：** 对！ 默认为SHA-256

<br> 

### 一般问题和评论：

<br> 

**问题：** 我们单击哪项可下载扩展名的源文件？ 这是在“3点菜单”中吗？

**回答：** 是！ 这3个圆点，然后“下载源”（从目录视图）

<br> 

**注释：** 对于扩展，我真正感兴趣的一点是它们的省时特性。 他们中的很多人做你做的事 *可以* 有一些自定义代码，但是使用扩展时，您无需编写该代码。

**回复：** 好极了。 它可重复使用，无需每次都重新创建轮子。

<br> 

**问题：** Web SDK实施将如何支持或替换Analytics插件？

**回答：** 现在，由于工作区和Adobe标记增加了灵活性，因此实际上无需使用许多Analytics插件。 但是，那些尚未迁移的用户正在积极迁移以供Web SDK使用。

<br> 

**问题：** 使用Web SDK跟踪Activity Map是否有任何开发？

**回答：** 我很高兴地报告，我们正在积极制定Activity Map以获取Web SDK中的支持

<br> 

**问题：** 在将事件传输到最终目标之前，我们是否可以访问Adobe Edge网络来管理事件？ 我了解我们也可以在Launch中这样做，但将来是否也可以在服务器上执行此操作？

**回答：** 是！ 这可以通过我们的事件转发功能实现，客户可以通过我们的任何Real-Time CDP产品(Real-Time CDP Connections、Prime或Ultimate)购买该功能。

**回答：** RTCDP连接（事件转发）让您在将连接发送到非Adobe目标之前拥有更多控制权。

**回答：** 查看我们的一些其他ExL Live视频以了解更多相关信息(例如 [这个](exl-live-episode-06-23-22.md))。

<br> 

**注释：** 快速调用我最喜爱的扩展之一：有一个映射表扩展，您可以在其中为“如果此值是这个，则将其设置为那个”的数据元素读取表。

**回复：** 它们提供的灵活性令人印象深刻。 还需要注意的是，公司也可以自行创建私有扩展。

<br> 

**问题：** 您显示了来自CRM的单个数据，如城市和天气，那么我们要将单个响应存储在何处？

**回答：** 响应存储在触发事件转发属性中规则的每个唯一事件中，并且仅用于该特定事件。

<br> 

请继续在 [Experience League社区讨论](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## 此数据收集系列中的其他Experience League实时会话

* [咨询专家 — Web SDK基础知识](exl-live-episode-05-26-22.md)
* [询问专家 — RTCDP连接](exl-live-episode-06-23-22.md)
* [咨询专家 — 数据流和数据准备](exl-live-episode-07-21-22.md)
