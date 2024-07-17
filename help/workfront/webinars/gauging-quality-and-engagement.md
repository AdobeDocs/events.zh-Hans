---
title: 咨询专家 — 评估质量和参与度
description: 了解如何构建可回答质量和参与度问题的报表。 该网络研讨会于2019年11月13日录制。
doc-type: feature video
team: Technical Marketing
kt: 9914
exl-id: 76a8e418-71c7-414a-9938-e64e4e73c184
duration: 3980
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---

# 咨询专家 — 评估质量和参与度

了解如何构建可回答质量和参与度问题的报表。 该网络研讨会于2019年11月13日录制。

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## Q&amp;A

**问题**

有一些字段可供筛选，但在您尝试按这些字段进行分组时不可用。 您是否正在努力使其成为一致的选项？

**答案**

报告工具不允许您按动态字段或可一次选择多个选项的字段进行分组，例如复选框字段。 您只能对具有单个值的字段进行分组，即使它们可能有多种选择。

您可以按复选框进行筛选和查看，只是不能对它们进行分组。

**问题**

在作业角色迭代示例中，能否以粗体显示主要角色？

**答案**

在迭代中，我们可以确定主要工作角色。 我们需要在valueexpression中执行这项操作，但在valueexpression中无法识别HTML代码。 所以我们需要想出另一种方法，将角色确定为主要角色。 在此代码中，我将“**”放在主要角色名称之前和之后。 尝试一下，看看您喜欢的程度：

```
displayname=All Job Roles 
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("**",{role}.{name},"**"),{role}. {name})
valueformat=HTML
```

这将为您提供如下列表：

```
Support Engineer 
QA Engineer 
**Designer**
```

其中Designer是此用户的主要角色。

**问题**

嗨！ 我正在为我们的编辑团队整理一个工作流，以跟踪文章在其生命周期中的位置（初始写入 — >部门审核 — >最终编辑 — >发布）。 他们想要轻松查看当前所处的里程碑或任务。 我收到的反馈是标准的“里程碑”视图（使用红色或绿色阴影）太“忙且复杂”。 能否在表或网格中仅显示“项目名称”和“当前里程碑”？

**答案**

可以。您可以创建一个任务报告，以显示当前正在处理的里程碑任务以及与其关联的任务。 您可以在表格或列表报告中执行此操作。

**问题**

能否在报告中将验证信息与项目信息相结合？

**答案**

如果已创建验证审批报告，则可以使用文本模式将项目信息拉入列。 例如，如果您想在列中引用项目名称，则可以使用以下命令：

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**问题**

我还想了解有关报告与项目相关的证明数据的更多信息。 例如，包含验证决策和评论的项目报告。

**答案**

要在单个报告中引用项目信息和验证信息，您需要创建验证审批报告。 目前，无法将来自验证的评论提取到此报告中，但是，可以在“审批者决策”列下的单独行项目中找到每个验证审批者决策。

**问题**

我经常使用sharecol来创建单页面状态（多列）。 但是，我发现在创建报告后，如果我想在页面顶部添加列，则返回并进行修改会非常耗时。 您是否有任何进行此类更改的提示或技巧？

**答案**

如果您正在讨论将列放在文本模式列列表的顶部，则只需手动为列重新编号。

但是，如果您已经创建了报告，其中第一列是一些共享列，并且您想将另一个共享列放在列表顶部，这比较容易。

在报表编辑器中，只需添加几个新列，然后将它们拖动到“列（视图）”屏幕的最左侧。 执行此操作后，请查看以前位于左列的内容，您会注意到文本模式的列号均已递增。 根据需要将任意数量的空白列拖动到那里。 保存前，请确保将某些内容放入这些空白列中，否则它们将被去除。

**问题**

您好 — 关于最终错误报告 — 如何为多个项目创建报告 — 如果多个项目中出现错误??

**答案**

您可以按项目组合或项目进行过滤，具体取决于您组织工作的方式。

您还可以根据请求队列进行过滤。 您可能需要为每个项目设置请求队列，您可以将客户用户创建为审阅者，审阅者可以直接登录并将票证提交到您与他们共享的请求队列。

**问题**

第一个报告基于项目/项目名称，这是否也基于任务完成，如果是这样，那么分组它们的最佳方式是尽可能使任务名称频繁地不同……谢谢！

**答案**

所有这些报告都可以作为任务、问题或项目报告来完成，具体取决于您决定如何跟踪这些内容。

对任务进行分组的常见方法是先按其项目名称对任务进行分组，然后按每个项目中的任务名称对任务进行分组。 这样一来，如果您有两个具有相同名称的任务，则很容易看到它们所在的项目。

**问题**

我想了解哪些校样是突出的，它们与什么任务和项目相关联，何时路由，何时到期，以及谁是审查方和批准方。

**答案**

未完成的校样可以通过等待决策>等于>校样审批报告中的True进行过滤。 有一列“审批者”将告诉您谁尚未做出决策。

您可以使用文本模式引用验证绑定的任务或项目（请参阅下面的示例）。

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name
valueformat=HTML
```

至于发送日期、截止日期和审查方，这些字段目前无法拉入任何Workfront报表，因此您需要直接单击验证以查看该信息。

**问题**

能否设置自定义表单，以便在请求者完成请求后自动发送给请求者？ 比如说一项“客户满意度”调查？

**答案**

有一件事你可以做，也许能满足你的需要。 您可以向问题附加提醒通知，该问题将在输入实际完成日期后向“输入者”发送电子邮件。 输入者是创建问题的人员。

您可以创建提醒通知，就像我们在“提醒填写行动后审核(AAR)”的网络研讨会中所做的那样，只不过这里是一个问题提醒。 您可能还希望为其创建一个电子邮件模板，以提供调查链接。 您必须手动将提醒通知应用于每个问题（或使用批量编辑）。

集成会更好，因为它可以自动执行手动步骤，但提醒通知可以立即完成。

**问题**

我创建了一个报表，其中按模板类型显示了项目。 我可以列出项目所有者，但不能列出分配给项目的人员。

**答案**

如果要将“项目团队”（“人员配备”选项卡）拉入项目报告中的列，则需要通过文本模式创建此列。 文本模式如下所示：

```
displayname=Staffing 
listdelimiter=<p> 
listmethod=nested(projectUsers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

## AAR参与报表的文本模式代码

```
column.0.displayname=Task Details
column.0.value=<b>Project Name:</b>&nbsp;
column.0.valueformat=HTML
column.0.sharecol=true
column.1.valuefield=project:name
column.1.valueformat=HTML
column.1.sharecol=true
column.2.value=<br>
column.2.valueformat=HTML
column.2.sharecol=true
column.3.value=<b>Task Name:</b>&nbsp;
column.3.valueformat=HTML
column.3.sharecol=true
column.4.valuefield=name
column.4.valueformat=HTML
column.4.sharecol=true
column.5.value=<br>
column.5.valueformat=HTML
column.5.sharecol=true
column.6.value=<b>Task Owner:</b>&nbsp;
column.6.valueformat=HTML
column.6.sharecol=true
column.7.valuefield=assignedTo:name
column.7.valueformat=HTML
column.7.sharecol=true
column.8.value=<br>
column.8.valueformat=HTML
column.8.sharecol=true
column.9.value=<b>Actual Completion Date:</b>&nbsp;
column.9.valueformat=HTML
column.9.sharecol=true
column.10.valuefield=actualCompletionDate
column.10.valueformat=HTML
column.11.displayname=Name of Reviewer
column.11.linkedname=Name of Reviewer
column.11.namekey=view.relatedcolumn
column.11.namekeyargkey.0=Name of Reviewer
column.11.namekeyargkey.1=name
column.11.querysort=DE:Name of Reviewer:name
column.11.valuefield=Name of Reviewer:name
column.11.valueformat=customReferenceObjectAsString
column.12.displayname=AAR 1
column.12.description=In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.12.value=<b>AAR 1 Score:</b>&nbsp;
column.12.valueformat=HTML
column.12.sharecol=true
column.13.valuefield=AAR 1 - In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.13.valueformat=customDataLabelsAsString
column.13.sharecol=true
column.14.value=<br>
column.14.valueformat=HTML
column.14.sharecol=true
column.15.value=<br><b>AAR 1 User Comment:</b>&nbsp;
column.15.valueformat=HTML
column.15.sharecol=true
column.16.valuefield=AAR 1 User Comment
column.16.valueformat=customDataLabelsAsString
column.17.linkedname=direct
column.17.namekey=AAR 1 Reviewer Comment
column.17.querysort=DE:AAR 1 Reviewer Comment
column.17.valuefield=AAR 1 Reviewer Comment
column.17.valueformat=customDataLabelsAsString
column.18.linkedname=direct
column.18.displayname=AAR 1 Needs Attn
column.18.querysort=DE:AAR 1 Needs Attention
column.18.valuefield=AAR 1 Needs Attention
column.18.valueformat=customDataLabelsAsString
column.19.linkedname=direct
column.19.displayname=AAR 1 Needs Attn Notes
column.19.querysort=DE:AAR 1 Needs Attention Notes
column.19.valuefield=AAR 1 Needs Attention Notes
column.19.valueformat=customDataLabelsAsString
column.20.displayname=AAR 2
column.20.description=Do You Believe This Work Will Make an Impact?
column.20.value=<b>AAR 2 Score:</b>&nbsp;
column.20.valueformat=HTML
column.20.sharecol=true
column.21.valuefield=AAR 2 - Do You Believe This Work Will Make an Impact?
column.21.valueformat=customDataLabelsAsString
column.21.sharecol=true
column.22.value=<br>
column.22.valueformat=HTML
column.22.sharecol=true
column.23.value=<br><b>AAR 2 User Comment:</b>&nbsp;
column.23.valueformat=HTML
column.23.sharecol=true
column.24.valuefield=AAR 2 User Comment
column.24.valueformat=customDataLabelsAsString
column.25.linkedname=direct
column.25.namekey=AAR 2 Reviewer Comment
column.25.querysort=DE:AAR 2 Reviewer Comment
column.25.valuefield=AAR 2 Reviewer Comment
column.25.valueformat=customDataLabelsAsString
column.26.linkedname=direct
column.26.displayname=AAR 2 Needs Attn
column.26.querysort=DE:AAR 2 Needs Attention
column.26.valuefield=AAR 2 Needs Attention
column.26.valueformat=customDataLabelsAsString
column.27.linkedname=direct
column.27.displayname=AAR 2 Needs Attn Notes
column.27.querysort=DE:AAR 2 Needs Attention Notes
column.27.valuefield=AAR 2 Needs Attention Notes
column.27.valueformat=customDataLabelsAsString
column.28.displayname=AAR 3
column.28.description=Are you proud of the work you did on this?
column.28.value=<b>AAR 3 Score:</b>&nbsp;
column.28.valueformat=HTML
column.28.sharecol=true
column.29.valuefield=AAR 3 - Are you proud of the work you did on this?
column.29.valueformat=customDataLabelsAsString
column.29.sharecol=true
column.30.value=<br>
column.30.valueformat=HTML
column.30.sharecol=true
column.31.value=<br><b>AAR 3 User Comment:</b>&nbsp;
column.31.valueformat=HTML
column.31.sharecol=true
column.32.valuefield=AAR 3 User Comment
column.32.valueformat=customDataLabelsAsString
column.33.linkedname=direct
column.33.namekey=AAR 3 Reviewer Comment
column.33.querysort=DE:AAR 3 Reviewer Comment
column.33.valuefield=AAR 3 Reviewer Comment
column.33.valueformat=customDataLabelsAsString
column.34.linkedname=direct
column.34.displayname=AAR 3 Needs Attn
column.34.querysort=DE:AAR 3 Needs Attention
column.34.valuefield=AAR 3 Needs Attention
column.34.valueformat=customDataLabelsAsString
column.35.linkedname=direct
column.35.displayname=AAR 3 Needs Attn Notes
column.35.querysort=DE:AAR 3 Needs Attention Notes
column.35.valuefield=AAR 3 Needs Attention Notes
column.35.valueformat=customDataLabelsAsString
column.36.displayname=Done
column.36.valuefield=Review Complete
column.36.valueformat=customDataLabelsAsString
```
