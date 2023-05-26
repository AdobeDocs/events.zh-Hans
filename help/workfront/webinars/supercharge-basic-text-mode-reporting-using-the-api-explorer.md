---
title: 咨询专家 — 使用API Explorer进行超额基本文本模式报告
description: 了解API Explorer及其使用方法，以及如何利用基本文本模式增强报表。 该网络研讨会于2020年1月22日录制。
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9918
exl-id: ea4716c9-2c61-4c44-9d2a-cbd4f07699d5
source-git-commit: ca06e5a8b1602a7bcfb83a43f529680a5a96bacf
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 2%

---

# 咨询专家 — 使用API Explorer进行超额基本文本模式报告

了解API Explorer及其使用方法，以及如何利用基本文本模式增强报表。 该网络研讨会于2020年1月22日录制。

>[!VIDEO](https://video.tv.adobe.com/v/341124/?quality=12)

## 其他资源

![显示文本模式代码规则示例的图表](assets/text-mode-chart.png)


**最后“所有工作角色”列**

```
description="Primary =" indicates the user's primary job role
displayname=All Job Roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("Primary = ",{role}.{name}),{role}.{name})
valueformat=HTML
```

**“所有团队”列的文本模式**

```
displayname=All Teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

**“所有组”列的文本模式**

```
displayname=All Groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

**“直接下属”列的文本模式**

```
displayname=Direct Reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

## Q&amp;A

**问题**

是否可以使用文本模式在报表中使用任何收藏集？

**回答**

可以，您可以使用收藏集中的任何对象。 您需要浏览并查看您有权访问的内容。 并非所有对象都具有对用户对象和工作角色对象的访问权限，就像我们在API资源管理器中使用用户角色对象时看到的那样。

**问题**

能否讨论“同一列中不同收藏集的条件使用（项目更新与任务更新）”

**回答**

当处于迭代区域并在其中看到valuefield或valueexpression时，即表示正在访问收藏集列表中的项之一。 例如，通过使用valuefield，我们可以获取该工作角色的名称，或列表中该项中的任何内容。 如果您在任务中，任务对象可以引用它所在的项目。

**问题**

能否讨论“任务更新集合是否只能在任务报告中使用？”

**回答**

创建问题报告时，您可以查看任务信息（如果针对任务报告了问题），还可以从收藏集中查看该信息。 除了这些情况，您需要在任务报表中查看任务收集数据。

**问题**

能否共享文本格式([!DNL CSS])示例？

**回答**

Workfront不支持 [!DNL CSS] 在文本模式下。

**问题**

对于文本模式报表，找到自定义字段名称的最佳或最快方法是什么？ 我已在浏览器中使用“HTML编辑”选项，方法是在报表中添加字段并切换到文本模式以抓取该字段，但……好奇其他人如何执行此操作

**回答**

我发现在UI中选择字段，然后切换到文本模式并复制字段名称是最快的方法。 这确保我获得字段的正确拼写。

**问题**

如何使用文本模式在报告中标识团队成员？ 我们当前在任务审批工作流中使用团队分配，并希望在当前审批阶段中将团队成员列在一个类似于“审批者和状态”字段工作方式的列中。

**回答**

要引用与当前审批阶段关联的团队成员，您需要引用引用集合的集合，而当前通过Workfront的文本模式功能无法实现此功能。 您的组织当前使用的列（显示与批准关联的团队）是您的最佳选项。

**问题**

字段和对象名称是否必须为大小写(例如， 角色与角色)？

**回答**

当您在文本模式下引用对象时，您将希望其编写方式与API Explorer右侧列显示的完全相同。 例如，如果要从“任务”报表中引用项目名称，则valuefield如下所示：

```
valuefield=project:name
```

但是，对于问题，这些任务在API Explorer中称为opTasks。 因此，如果您要运行小时报告，并想要为问题名称添加列，则valuefield将如下所示：

```
valuefield=opTask:name
```

**问题**

我希望构建一份报告，显示每个项目的当前活动任务。 我该怎么做呢？ 我猜想它会是一个任务报告，并且还添加了项目信息列？

**回答**

没错。 最好是编制一份任务报告。 您需要定义“活动任务”。 如果您使用的是前置任务，则这些任务已经就绪。 因此您可以按Ready = True进行过滤。 这将产生任何已准备好开始的任务。 然后，我建议您按项目名称分组，这样可以将您的任务都分组在一起，并且您可以一眼就看到哪些任务属于哪个项目。

**问题**

是否有办法创建可计算数据（例如，满足特定标准的项目百分比）的报表？

**回答**

创建报表以显示或计算数据（例如%）的最佳方法是将分组应用于报表，然后应用图表。 如果要在报表中添加饼图，可以选择饼图扇区的值或百分比。

**问题**

是否可以使用文本模式标识分配给当前任务审批阶段的团队成员，这与“审批者和状态”列类似？

**回答**

您需要在“任务”报表中添加一个以文本模式显示的收藏集列，该列具有以下内容：

```
displayname=Current Approval Stage Approvers 
listdelimiter=<p> 
listmethod=nested(currentApprovalStep.stepApprovers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

**问题**

能否筛选所有组包含特定组的位置？

**回答**

如果要筛选报告中的项目，请在报告的筛选选项卡下执行此操作。 因此，如果您希望仅查看其群组之一为记帐的用户，则可以添加一个过滤器规则，其中显示：

```
Other Groups>ID>Equal>Accounting
```

**问题**

是否可以通过创建报告来确定任务组合的实际持续时间？

**回答**

您需要对报表进行筛选，使其仅包含所需的任务组合。 然后，您需要将“实际持续时间”列放入视图中，并在“列设置”中按“总和”进行汇总，最后，您需要以某种方式将报表分组。 运行报告时，分组栏将显示分组行中包含的实际总持续时间。

**问题**

是否有办法减去父级下的任务，以确定父级下其余任务的持续时间？

**回答**

计算父级任务持续时间的方法是：从父级下最晚结束任务的结束日期减去最早开始任务的开始日期。 在报表中，您只知道考虑是否要显示的每个单独任务。 报表引擎无法保留一个任务中的信息并在查看另一个任务时使用它。 因此，要完成您所要求的任务，唯一的方法是在项目任务列表中删除处于某个父级下的任务，并观察如何重新计算父级任务的持续时间。

**问题**

对于条件分组，一种用于解码各个分组的自定义表单（例如“西部州”、“中部州”、“东部州”）是一种常用的技术，可在何时使用计算分组与计算参数时很好地应用于该注释？

**回答**

计算分组（也称为分组中的值表达式）是一种便于在分组栏中显示结果的方式。 这也可以使用计算自定义字段来完成。 每种方法都有优点和缺点，包括：

* 每次刷新浏览器页面时都会计算值表达式。 这可能优于已计算的自定义字段，在编辑这些字段附加到的对象时，或者在批量编辑中重新计算已计算的字段时，或者在编辑自定义表单并选择“更新以前的计算”选项时，重新计算这些字段。
* 但是，不能在图表、条件格式或筛选器中使用值表达式。 您需要对这些字段使用计算自定义字段。

**问题**

是否无法将分组显示名称从“无值”更改为我们出于报告目的而选择的其他任何名称？ 换言之，它永远是“没有价值”？

**回答**

有一种方法可以将“无值”替换为其他内容。 假设您有一个按Portfolio名称分组的项目报告。 所有未分配给项目组合的项目将最终位于标题为的分组中：

```
Portfolio: Name: No Value
```

要更改此项，请在文本模式下编辑分组并替换此行：

```
group.0.valuefield=portfolio:name
```

行：

```
group.0.valueexpression=IF(ISBLANK({portfolio}.{name}),"Not in any Portfolio",{portfolio}.{name})
```

该分组现在将具有此标题：

```
Portfolio: Name: Not in any Portfolio
```

**问题**

是否存在用于跟踪未完成分配的参数，即：

1. 具有单个分配但未分配个人的任务，或
1. 具有多个分配的任务，这些分配至少有一个未分配的个人用于请求的角色

**回答**

这可以通过使用“任务报告”和筛选来完成

```
Assigned To ID > Is Blank and Role ID > Is Not Blank
```

这将拉入已分配给某个角色但未一定分配给某个特定用户的所有任务或问题。 您需要添加任务和问题名称的列，以查看任务属于哪个对象，如果按项目名称分组，则它应有助于保持其井然有序。

**问题**

Chuck，我忘记了，但您是否还记得在文本模式下将随后在悬停时呈现为工具提示的属性？

**回答**

description=允许您在鼠标悬停在列标题上时显示工具提示。

**问题**

我是否可以报告允许进行多个选择但只将第一个选择提取到报告中的复选框字段？

**回答**

可以。复选框字段中的选定选项全部位于一个字符串中，每个选项之间用逗号分隔。 您将使用SEARCH表达式来查找第一个逗号在复选框字段中的位置，然后将该索引与LEFT表达式一起使用，以显示从列表开头开始的字符数。 代码如下：

```
valueexpression=IF(SEARCH(",",{DE:Checkbox Field},0)>0,LEFT({DE:Checkbox Field},SEARCH(",",{DE:Checkbox Field},0)),{DE:Checkbox Field})
```

如果您在复选框字段的选项名称中使用逗号，则它将仅显示选定内容的部分，直到显示第一个逗号。
