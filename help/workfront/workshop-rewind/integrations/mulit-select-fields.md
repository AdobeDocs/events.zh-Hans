---
title: 轻松浏览Workfront API和针对多选字段的Fusion更改
description: 了解即将推出的Adobe Workfront API和Fusion更改，包括多选字段更新、事件订阅版本控制和防止重大更改的策略。
feature: Workfront API, Workfront Fusion, Workfront Integrations and Apps
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3172
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18631
source-git-commit: 6225f36c5d26ecca5ebc2aca24a2d592a3279570
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# 轻松浏览Workfront API和针对多选字段的Fusion更改

此研讨会录制于2025年6月25日，Andy Hess在会上介绍了即将对Workfront API和Fusion所做的更改。

>[!VIDEO](https://video.tv.adobe.com/v/3469978/?learn=on&enablevpops)

## 资源

除了按需录制之外，我们还包含幻灯片和其他资源：
* [幻灯片组PDF](https://workfront-experience.s3.us-west-2.amazonaws.com/Training/Guides/Customer+Success+at+Scale/Navigating+the+API+and+Fusion+Changes+for+Multi-Select+Fields+with+Ease+062425.pdf)
* 与Adobe软件开发团队合作主办的活动已在5月初交付，如果您想了解有关该特定领域的更多信息，[[事件跟进]在事件订阅V2升级期间保留您的融合方案](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/m-p/754182#M4041)

## 主要任务和资源

* 版本21（2025年10月）将对Workfront API多选字段进行更改，以确保一致的JSON数组格式而不是混合字符串/数组响应
* 正在引入事件订阅版本控制 — 版本2将始终将多选字段作为数组返回，而版本1保持当前不一致行为
* 新事件订阅会自动默认使用版本2，并且所有订阅将在2026年1月中旬自动升级到版本2
* 新的Workfront连接器版本将在今年晚些时候发布，其中包含手动升级过程，以保留模块映射并防止重大更改
* Fusion AI助手当前可用，但需要签订的AI协议和正确的许可设置。 如果您有问题或想了解更多信息，请联系您的客户经理。 [有关在Fusion中使用AI的更多信息](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/manage-scenarios/fusion-ai-assistant)
* [当前可用的Workfront Fusion模板](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/create-and-manage-templates/currently-available-fusion-templates)
* [调用Fusion模板](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/call-for-fusion-template-ideas/m-p/732085#M3686) — 如果您有新Fusion模板的建议，请在此处添加这些建议！ 团队可以从这里获取想法  

如果您有任何后续问题，请回复此[Experience League社区帖子](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-navigating-the-workfront-api-and-fusion-changes/td-p/761253)！ 

我们希望在未来的客户成功研讨会上与您见面！  请务必查看Experience League上的[Workfront活动](https://experienceleague.adobe.com/events/?lang=zh-Hans&filters=Workfront)以获取完整列表并注册。