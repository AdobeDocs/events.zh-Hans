---
title: Marketo和Mochas - Salesforce同步
description: 通过权限、字段可见性、管理员协作和最佳实践方面的专家指导，掌握Marketo-Salesforce同步，以确保流畅、优化的集成。
feature: Salesforce Integration
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3547
last-substantial-update: 2025-08-07T00:00:00Z
jira: KT-18706
source-git-commit: bc5752512fb1bc50cefe0180c308574e821888a2
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# Marketo与Mochas：Salesforce同步

Marketo只有非常少的本机集成，但Salesforce是其中功能最强大的。 鉴于约90%的Marketo客户也在使用Salesforce，Adobe致力于向客户提供有关如何理论、诊断和优化两者之间同步的建议。 Marketo与SFDC的同步主要基于SFDC中授予Marketo同步用户的权限。 由于多个管理员或不同的团队围绕系统中的更新创建通信孤岛，因此客户可能很难做到这一点。

此网络研讨会包括以下与Marketo &lt;-> SFDC同步相关的内容：

·以鸟瞰的方式解释同步的工作原理
·在SFDC中从Marketo同步用户隐藏字段和对象
·如何与SFDC管理员通信
·如何与Marketo支持部门有效合作
·将Marketo同步到SFDC时应避免的事项

>[!VIDEO](https://video.tv.adobe.com/v/3470624/?learn=on&enablevpops)

## 使用Salesforce Sync的最佳实践

要有效地将Salesforce与Marketo同步，请遵循以下最佳实践，这些最佳实践逐步（用简单的术语说明）：

1. **了解同步过程**

   该同步操作会将Marketo与Salesforce连接起来，以便数据在两个系统之间流动。 可以将“Marketo同步用户”视为两个平台之间的桥梁。 此用户具有读取和写入特定数据的权限：

   * **写入权限**&#x200B;潜在客户和联系人(Marketo可以在Salesforce中更新这些联系人)。
   * **读取权限**&#x200B;帐户、商机、自定义对象和活动(Marketo可以查看这些内容，但不能更改它们)。

   当数据在Salesforce或Marketo中更改时，该同步每5分钟更新一次另一个系统。 但是，您可以使用诸如“同步到SFDC”之类的流程步骤来优先处理紧急更新。

1. **清理字段**

   仅同步正在使用的字段。 例如：

   * 如果您具有不再相关的旧字段，例如“COVID-19注释”，请从同步中删除它们。 这样可以减少杂乱情况并加快处理过程。
   * 避免同步公式字段（例如，“提前天数”），因为它们不更新时间戳，这可能会导致问题。

1. **防止积压**

   当等待同步的数据过多时，会发生积压。 要避免这种情况：

   * 限制不必要的更新：例如，如果帐户得分略有变化（例如，从60到61），则可能会触发所有相关联系人的更新。 相反，将分数分组到范围（例如，0-25、26-50）中以减少更新。
   * 批量营销活动：使用批量营销活动而非触发营销活动来更有效地处理数据。

1. **管理错误**

   当Marketo尝试更新Salesforce中的字段但没有权限时，可能会发生错误。 要进行故障排除：

   * 以Marketo同步用户身份登录Salesforce，然后尝试执行相同的操作。 这有助于识别权限问题或无效数据。
   * 在Marketo中设置循环活动以修复常见错误，例如对国家/地区值/州值进行标准化（例如，“CA”到“加利福尼亚”）。

1. **使用自定义同步筛选器**

   自定义筛选器可帮助您控制哪些记录在Salesforce和Marketo之间同步。 例如，创建一个名为“Do Not Sync to Marketo”的字段。 如果此字段在记录中标记为“true”，则不会同步到Marketo。 这对于排除无效的电子邮件地址或过期的联系人非常有用。

1. **限制任务创建**

   埃尔姆·Salesforce。 关注有意义的活动，如“填写的表单”或“电子邮件中的点击链接”。

1. **与您的Salesforce管理员协作**

   由于同步涉及两个系统，因此请与Salesforce管理员密切合作，以：

   * 管理Marketo同步用户的权限。
   * 清理Salesforce中不必要的字段。
   * 同步问题疑难解答。

1. **监视器同步性能**

   在Marketo的“管理员”部分中定期检查同步状态：

   查找“同步积压趋势”或“同步吞吐量”功能板中的峰值。 这些指示延迟或过度更新。
如果您发现问题，请调查哪些字段或记录导致了问题。

1. **明智地使用自定义对象**

   自定义对象是可存储其他信息（如产品详细信息）的特殊数据结构。 仅同步营销活动所需的自定义对象，以避免数据库膨胀。

1. **扩展性计划**

   在设置同步时，请考虑长远因素：

   * 维护数据字典，以跟踪已同步的字段及其原因。
   * 避免同步不必要的字段或记录，以保持系统高效。

通过执行以下步骤，您可以确保Marketo与Salesforce之间平稳、高效的集成，从而最大限度地减少错误并最大化数据的价值。
