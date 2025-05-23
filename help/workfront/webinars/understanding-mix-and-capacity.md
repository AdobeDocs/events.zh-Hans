---
title: 咨询专家 — 了解混合和容量
description: 了解如何衡量企业内的混合和容量。 该网络研讨会于2019年10月2日录制。
doc-type: feature video
team: Technical Marketing
kt: 9913
exl-id: 49cce53f-457b-4973-a0d9-1b5ce2272884
duration: 4239
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '2230'
ht-degree: 0%

---

# 咨询专家 — 了解混合和容量

了解如何衡量企业内的混合和容量。 该网络研讨会于2019年10月2日录制。

>[!VIDEO](https://video.tv.adobe.com/v/341119/?quality=12)

## Q&amp;A

**问题**

如何将%s放在柱形图上？

**答案**

混合报表中列出的%值之所以存在，是因为我们在图表选项卡中选择了“组列”和“栈叠到100%”。 如果我们选择“栈叠”，则会显示计划小时数总计，而不是百分比。

**问题**

如果您的部门/组织工作负载是项目/任务和问题/请求的混合，您建议如何获得WPI的高级审核(在Workfront报表中)。

**答案**

项目、任务和问题需要各自具有带有其自定义表单的报表。 但是，它们可以各自使用相同的工作类型字段。 您可能希望在一个仪表板中显示三个报告。

**问题**

我们是否必须批量编辑任务以使它们具有可操作性或战略性？

**答案**

我们建议的技术是创建一份报告，让您获得可操作的任务列表。 一旦完成，您可以一次选择所有任务，批量编辑它们，然后附加具有“工作类型”的自定义表单，并将所有任务的工作类型设置为“可操作”。 您可以按照相同的流程收集策略任务的列表、批量编辑这些任务并添加自定义表单等。

网络研讨会中提到了一些自定义提示的想法，这些提示可能会帮助您获得列表，例如检查任务名称、项目所有者、项目组合或分配的用户中的特定词语。 这些只是想法。 您应该设计一份最适合您情况的报告。

**问题**

如果我的组合中包含4个类别，我能否为每个类别创建一个目标，然后报告预测与计划与实际之间的增量？ （营销活动、业务部门、Web和产品共4类）。 我们在项目级别有自定义表单/字段中的类别。 目标将是创建季度预测（预算/预测），然后跟踪计划小时数并最终达到实际值。

**答案**

如果您将所有类别都在一个自定义字段中（现在我们将其称为“工作类型”），则只需先创建按计划小时数分组的项目报告，再创建按工作类型分组的项目报告。 筛选项目报表，以在Planning中显示所需日期范围内的项目。 如果要查看百分比，请使用具有分组的列或栈叠到100%的条形的图表。 这可以是您的Forecast报告。

您可以复制报告并编辑它以根据当前项目创建报告，仍根据计划小时数显示组合。

您可以再次复制报表，将其更改为按实际小时数而不是计划小时数分组，并仅显示所需日期范围内的已完成项目。 这将显示基于实际小时数的百分比组合。

**问题**

如果您在项目或任务中具有多个类别ID，此功能是否有效？

**答案**

能，如果您有多个ID，则需要用制表符分隔，如下所示：

```
EXISTS:1:$$EXISTSMOD=NOTEXISTS
EXISTS:1:$$OBJCODE=OBJCAT
EXISTS:1:categoryID=5d76d82600e7926bb51eeb1e0886810e 5d54288d01034619f2eb2c74f6472f18
EXISTS:1:objID=FIELD:ID
```

使用制表符将它们分隔开的最佳方法是先在生成器中创建类别列表。 输入多个自定义表单名称，当您切换到文本模式时，您会看到它们是以制表符分隔的ID。

多个ID都将被视为OR，因此其中任何一个附加到任务的ID都不会显示在报表中。

**问题**

报表提示是“与”还是“或”？

**答案**

单个自定义提示为“ANDed”。 因此，如果您将Pam指定为项目责任人，将Bill指定为任务分配人，则您只会看到在Pam为项目责任人的项目中分配给Bill的任务。

**问题**

为什么只能按特定列排序？ 即您不能按任务排序。

**答案**

“任务”是一个列表，您不能在项目列表中排序或分组。 您只能对单个项目进行排序或分组。

为了说明这一点，请设想一个任务中类似这样的任务列表：

```
Jane
Bill
Dan
```

另一个任务中的类似任务列表：

```
Bill
Jane
Helen
```

在排序中应该首先显示哪个任务？ 您可以说“按列表中的名字排序”，但这并不一定有用，因为您无法控制顺序。 Workfront不允许您按列表进行排序，从而避免出现此问题。

按列表分组如何？ 如果我们可以按名称列表分组，您将找到分配给Jane、Bill、Dan的所有任务分组在一起，以及分配给Jane、Dan和Bill的所有任务（同一列表，但顺序不同）在不同的分组中。 同样，Workfront通过不允许按列表分组来避免该问题。

**问题**

计划小时数是否用于战略任务，实际小时数是否用于运行？

**答案**

不会。在我们的示例中，我们使用计划小时数来显示战略和运营任务的计划工作量。 这使我们能够轻松比较它们，无论是过去、现在还是将来。 您还可以使用实际小时数来比较战略任务和运营任务，但仅适用于过去的任务，因为实际小时数是人员报告的实际执行任务所用的时间。

**问题**

在资源规划程序中，我们如何考虑过去已规划但未完成的任务？ 计划的小时数似乎未前滚，因此，在未来几周内不会显示为需要资源的任务/小时数。

**答案**

未完成的工作没有“自动”前滚。 发生这种情况时，您需要重新计划项目。 也许您最初分配给某个任务的资源在新的时间范围内不可用，因此项目经理必须了解这一点并确定重新计划的最佳方式。 这可能意味着让利益相关者参与并为计划中的更改获取批准。

**问题**

您建议调整其FTE吗？而不是每天输入2小时来检查电子邮件、休息时间。

**答案**

是，如果您将FTE设置为。75，则在资源规划程序中将显示用户每天6小时的可用时间。 这是他们每天的可用时间。 如果要根据日期的不同将其显示为不可用（如每个季度的最后一天不可用），则间接费用项目是执行此操作的途径。

有些人更喜欢管理费用项目，因为他们可以自己构建项目并在需要时更改项目，而他们可能无权编辑自己的约当全职人数。

**问题**

无论您与谁共享报告，无论他们具有什么工作权限，团队容量功能板的数据是否都能供任何人使用？

**答案**

如果用户没有查看对象的权限，则该对象在报表/功能板中不可见。 但是，如果您希望每个人都看到相同的结果，您可以进入报表操作>编辑>报表设置，并在字段“使用此报表的访问权限运行此报表”中输入您的姓名。 这将允许在此报告上共享的用户查看您所看到的确切结果。 它不会授予用户访问结果本身的额外权限，因此某些结果可能不可点击，也可能不可点击。

**问题**

我们如何创建一个报告来显示整个项目的所有分派员工（不是在任务级别）？

**答案**

您可以在项目报告中创建一个列，该列显示作为“人员配备”选项卡（项目团队）的一部分列出的所有用户。 您将希望使用以下文本模式：

```
displayname=Project Team
listdelimiter=<p>
listmethod=nested(projectUsers).lists
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

**问题**

我希望有一个报告/仪表板，其中包含我的团队的工作方式。 特别是以下情景： — 我拥有的项目/为我创建的项目/我分配给其他人的任务/分配给我的任务

**答案**

我拥有的项目

有一个名为“当前项目”的内置报告，其中将显示所有当前项目。 您可以编辑此项目并添加筛选器规则：项目>所有者ID >等于> $$USER.IDT。然后保存报告并将其重命名为“我拥有的项目”。

为我创建的项目

这里有一个名为“我的项目”的内置报告，它将向您显示您目前在项目团队中的所有项目（这意味着您是所有者、发起者或任务负责人）。 不确定您是否正在要求这样做，但除了让您成为项目所有者、发起人或将您分派到任务外，没有其他方法知道是否有人为您创建了项目。

我分配给其他人的任务

创建包含任何所需过滤器的任务报告，然后转到“过滤器”选项卡，并单击“切换到文本模式”。 将此代码添加到已有的任何代码中：

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

这将显示登录用户至少分配了一个当前被分配人的所有任务。 如果多个人员分配了受分配人，则分配人员的第一个人员的姓名将在任务登陆页上显示为“请求者”。 如果您要查看所有已分配人员和已分配人员，可以向视图中添加列，切换到文本模式，然后将其中的内容替换为以下内容：

```
displayname=All Assignees and Requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

分派给我的任务

有一个名为“我的任务”的内置报告，它将向您显示您是任务负责人的当前项目中的所有未完成任务。 我建议您更改过滤器以显示您是可能分配了多个用户的其中之一的所有任务，而不仅仅是任务所有者。 您可以通过删除筛选规则来实现这一点

```
Task > Assigned To ID > Equal > $$USER.ID 
```

并将其替换为

```
Assignment Users > ID > Equal > $$USER.ID
```

**问题**

是否有自定义图表标签的方法？ 我发现，当我创建图表来反映项目状态时，主组的名称最终会包含在标签中。

**答案**

图表上的标签使用您要分组的字段名称。 因此，更改标签的唯一方法是将计算自定义字段用于所需的任何名称。 在字段的计算部分中，输入要作为分组依据的本机字段的字段名称。

**问题**

请问您如何对Chuck团队分配的报告栏进行颜色编码？ 即琥珀色代表后方，红色代表后方，绿色代表准时？ 您能否将顺序更改为更符合逻辑的顺序（即红色/琥珀色/绿色，还是反之）？

**答案**

要更改报告中用于“进度状态”选项的颜色，请编辑报告并单击“图表”选项卡。 查找“Custom Colors >”（自定义颜色>）下拉列表。 它将显示在“左(Y)轴”框或“数据分组依据”框旁边，具体取决于您选择的是对列还是条进行分组。 在该下拉菜单中，您可以选择颜色。 如果单击颜色选项右下方的数字，则可以从较大的调色板中选择颜色。

很遗憾，您不能更改这些项目的顺序。

**问题**

能否创建一个图表，使其指向工作人员在其中分配了任务的项目计数？

**答案**

是的，方法如下：

* 创建项目报告
* 如果相关用户是登录用户，则过滤器应包括以下行：

```
   Project Users > ID > Equal >$$USER.ID 
```

* 如果没有，则将用户名替换为[!DNL $$USER.ID]。 这将显示此用户被分配了任务或者是其所有者或发起人的所有项目。 如果您只想查看分配了任务的项目，则应该添加以下两个额外的筛选规则：

```
   Project > Owner ID > Not Equal > $$USERID
   Project > Sponsor ID > Not Equal > $$USERID
```

* 创建至少一个分组，以便创建图表。 任何事都分组，例如公司。 然后单击“图表”选项卡并选择图表。 “记录计数”将是一个轴的默认值。 这将是用户分配到的项目数。

当用户获得项目分配（分配给任务或项目所有者或项目发起人）时，该人员将添加到项目团队，并且可以在“人员”子选项卡下的“人员配备”选项卡中看到。 如果从项目所有者、发起人或具有任何任务分配中删除用户，则其名称仍保留在项目团队中。 如果您希望删除它，则必须手动将其删除。 请记住，这可能会影响报告结果的准确性。 要从项目团队中删除某人，请转到人员配备>人员，选择一个或多个人员，然后单击列表上方显示的“删除”按钮。

**问题**

如何在文本模式（在分组中）中更改列的降序顺序？

**答案**

在构建报表时，您可以选择对列（视图）选项卡中的大多数列进行排序。 如果您没有分组，这将对您的整个列表报告进行排序。 如果您有分组，则它将根据每个分组中的该选择排序。

**问题**

如何创建列来标识分配到审批阶段的团队成员？

**答案**

如果您正在运行“任务”或“问题/请求”报告，则Report Builder中有一个名为“批准者和状态”的列将纳入此信息。
