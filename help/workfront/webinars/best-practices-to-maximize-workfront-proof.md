---
title: 咨询专家 — 最大限度地发挥Workfront Proof作用的最佳实践
description: 了解如何在Proof中配置设置、启用优秀报告和避免常见隐患。 该网络研讨会录制于2020年2月26日。
doc-type: feature video
team: Technical Marketing
kt: 9916
exl-id: 7d3e437d-4a6e-44b8-9eff-eabb8284c391
duration: 5182
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '5572'
ht-degree: 0%

---

# 咨询专家 — 最大限度地发挥Workfront Proof作用的最佳实践

了解如何配置设置以取得成功，访问视图（和其他技巧）以实现出色的报告，并了解如何避免Proof中的常见陷阱。 该网络研讨会录制于2020年2月26日。

>[!VIDEO](https://video.tv.adobe.com/v/341122/?quality=12)

## Q&amp;A

**问题**

目前，为了让收件人能够共享与其共享的验证，您必须手动选中验证设置下的“订阅”框。 是否有计划默认自动选中此框？

**答案**

管理员可以将其作为默认启用/禁用个人用户，方法是遵循以下路径： PHQ登录>帐户设置>用户>单击用户的名称>默认验证设置。

**问题**

如果您未选择“新验证”并上传文档，则用户将设置为“自动生成验证”。 在文件上载后，您能否修改这些设置？

**答案**

可以。您可以通过选择文档选项卡中的校样，然后单击校样详细信息来调整所有校样设置。

**问题**

此演示文稿是否适用于独立工具？

**答案**

有关验证角色的Recommendations、电子邮件警报、决策选项、转发电子邮件以及工作流模板分组/共享/设置都与独立验证相关。

**问题**

您会将Proof模板用于什么用途？

**答案**

如果贵组织的内容审阅过程经常重复或内容经常由同一人员审阅，则可以创建包含审阅人的工作流模板，其中包含具有您指定的验证角色和通知设置的审阅人。

**问题**

什么是验证工作流模板？

**答案**

校样工作流模板是具有可应用于校样的预定校样路由工作流的模板。 利用它们，您可以实现验证审批流程的标准化和自动化。

**问题**

如何创建验证模板？

**答案**

作为管理员，您需要遵循以下路径： PHQ登录>工作流>新建>新模板。

**问题**

该模板共享功能是否允许与组和团队共享，还是仅允许与个人用户共享？

**答案**

此时您无法与Workfront“组”、“团队”、“工作角色”或“公司”共享工作流模板。 但是，您可以与个人共享它们，也可以与验证组共享。 要创建验证组，请按照以下路径操作：PHQ登录>组>新建组。

**问题**

在提交验证时（在组织下），是否有空间清理每个用户看到的文件夹，以便他们仅看到适用于他们的文件夹？ 而不是所有在公司帐户中创建的文件夹？

**答案**

此问题与Workfront Proof Standalone相关。 在独立的Workfront Proof中，您可以利用专用文件夹来隐藏文件夹，使其不被特定用户看到。 这将允许更精简地列出可从中进行选择的文件夹。 请注意，您还可以使用预先键入逻辑来查找要向其添加验证的文件夹。

**问题**

审阅人和批准者是否可以选择更改这些通知设置？

**答案**

Workfront中的管理员可以更改用户和联系人的默认电子邮件警报设置。 验证创建者随后可以在创建验证时更改通知设置以及其现有的验证。

验证收件人始终可以通过选择左侧菜单中的设置图标，在验证查看者工具中更改其验证级别的特定验证的电子邮件警报。

**问题**

电子邮件警报是否会覆盖全局通知？

**答案**

验证电子邮件警报完全独立于全局通知设置。

**问题**

如果审核者被设置为“已禁用”，他们如何知道是否有新的验证可供他们审核（如果他们拒绝了以前的验证）？

**答案**

电子邮件警报与新验证电子邮件、新版本电子邮件、风险电子邮件、延迟电子邮件和@Mentions电子邮件无关。 如果选择“已禁用”作为电子邮件警报，则您将只禁用有关活动的通知，例如评论、回复和验证决策(来自评论的@Mention电子邮件除外)。

**问题**

禁用电子邮件是否设置为企业范围？ 还是按Portfolio分类？

**答案**

位于设置>电子邮件>审阅和批准中的设置允许/禁止验证收件人发表评论时发送电子邮件，该设置位于企业范围（它是一个全局设置）。

**问题**

我有一个“访客”用户已添加到验证中，无法查看验证。 并且用户无权访问Workfront。

**答案**

如果访客可以访问验证，但不可以发表评论/做出决定，请确保检查他们在验证上的验证角色。 在这种情况下，他们可能已通过“只读”验证角色添加到验证中。 如果他们在验证中被设置为查看者或查看者和审批者，并且仍然无法发表评论/标记/决策，请提交支持票证。

**问题**

来宾用户是否需要许可证？

**答案**

访客用户不需要许可证。

**问题**

我看不到证明决策框吗？

**答案**

如果您在验证上没有看到验证决策框，则表示您可能已将验证设置为具有只读或查看者验证角色，或者您在验证中的阶段尚未开始。

**问题**

能否在WF>设置中阐明设置 — 如果您可以选择为每次评论发送电子邮件 — 即使PHQ中的电子邮件被禁用，也会发送这些邮件？ 谁会收到邮件??

**答案**

Workfront设置>电子邮件>审阅和批准通知选项与验证级别的电子邮件警报选项无关。 如果启用此项，则每个验证上的每个人都将在每次验证上的某人发表评论时收到一封电子邮件。

**问题**

之前，您建议为验证所有者以外的电子邮件警报“禁用”。 在这种情况下，收件人是否仍会收到电子邮件通知，告知他们已分配验证？

**答案**

可以。电子邮件警报（可以设置为所有活动、已禁用、决策等）与验证通知电子邮件(新验证、新版本、风险验证、延迟验证@Mentions)无关。

**问题**

如果您有一个实例，其中将某人添加到验证中，并且他们觉得不应出现在验证中，该怎么办？ 删除“不相关”不会为他们提供可选择的选项吗？

**答案**

这非常适合用于“不相关的决策”选项。 但是，如果某人不应出现在验证中，我建议他们在验证评论中@Mention到验证所有者，并请求将其删除。 如果应对验证做出决定的人员应当“不相关”地做出决定，而他们应当“已批准”或“需要更改”，则这可能会改变应用于该验证的工作流的工作方式。

**问题**

可在何处找到来宾用户“需要登录”复选框？

**答案**

创建验证时，这将位于验证创建页面上的验证设置中。 如果验证已创建，您可以通过选择文档选项卡中的验证并单击验证详细信息>设置来访问此设置。 请注意，您只能与拥有校对许可证的人共享需要登录的校对。

**问题**

如果某人将自己添加到验证中，是否可以将自己从验证中删除？

**答案**

如果人员拥有编辑权限，可以证明他们已被添加到中，则可以自行移除。 具有“编辑”权限的用户将是具有“管理员”或“主管”级别验证许可证的Workfront用户，以及具有“作者”或“审查方”验证角色添加到验证的人员。 任何其他人都需要由具有编辑权限的用户删除。

**问题**

为什么我会使用文档审批与验证审批，反之亦然？

**答案**

“文档审批”可用于不需要与要审批的文档内联的注释和标记的文档。 例如，我只需要您查看此文档，然后批准或拒绝它。 校样将允许在校样查看器工具中的文档中存在注释和标记。 例如，我需要您查看此验证、添加评论、添加标记并做出决定。 将来，计划是将两项功能统一起来，因为它们非常相似。

**问题**

我们是营销部门，并且进行了内部验证审批，然后需要向外部发送请求者。 我们不向请求者授予访问我们项目的权限。 我们也不希望他们在内部验证中看到我们的所有评论。 现在，我们正在制作新的干净校样，下载并通过电子邮件发送给他们。 我们希望他们使用Proof HQ，但不确定如何通过授予他们访问我们的项目的权限来实现这一点。 有什么建议吗？

**答案**

我建议使用自动化工作流模板，这将允许您使用“专用阶段”。 专用阶段允许您隐藏其他阶段中来宾审阅人的注释、标记和决策。 这将允许外部请求者完全隐藏您的内部验证查看。

**问题**

其他人创建验证后，将您自己添加为审阅者和审批者的最佳方式是什么？

**答案**

如果您是拥有管理员或主管验证权限的Workfront用户，则可以将自己作为查看者和审批者添加到您有权访问的任何验证。 否则，您将需要验证所有者（或拥有验证编辑权限的其他人员）为您添加。

**问题**

我们尝试了在验证中标记用户，但他们不会收到电子邮件通知。 帐户设置中是否有任何内容可确保发送电子邮件？

**答案**

我建议检查电子邮件过滤器/垃圾邮件文件夹以查看通知是否已发送到该文件夹，然后在电子邮件应用程序中进行必要的调整以将这些电子邮件列入白名单。 您还可以联系我们的支持团队以获得这方面的帮助。

**问题**

你只能@有证明许可证的人，对吗？ 与一样，此人从未出现在验证中，您希望为其添加标签(@)。

**答案**

如果您是访客或具有Manager的验证许可证的Workfront用户，则可以@Mention证验证中的任何人（无论此人是否拥有许可证）。 如果您是拥有主管或管理员验证许可证的Workfront用户，或者您是验证所有者，则可以@Mention验证平台中联系人列表中的任何人。

**问题**

此处的最大问题：电子邮件%2B寻址（电子邮件地址重复）。 这种情况为何发生，又如何发生，以及如何加以补救？

**答案**

如果某人使用错误的电子邮件地址手动将某人添加到验证中，则可能发生这种情况。 如果您遇到这种情况，管理员可以按照以下路径从Proof帐户中删除不正确的电子邮件地址： PHQ登录>联系人>选择不正确的电子邮件/来宾实例>删除。 如果您在添加具有重复电子邮件地址的用户时遇到问题，请联系我们的支持团队以获取帮助。

**问题**

做出决定后，您必须将验证更改回生产环境。 您需要授予生产团队哪种访问权限，以便他们在验证锁定后可以使用评论的操作？

**答案**

如果验证已锁定，则需要解锁该验证，用户才能处理评论或回复评论。 具有以下权限的用户可以解锁验证：验证所有者、具有管理员或主管级别的“验证许可证”的Workfront用户。

**问题**

团队了解人员队列中已存在的验证的最佳解决方案是什么？

**答案**

您可以在Workfront中创建验证审批报告。 然后，您可以应用过滤器以仅显示仍需要做出决策的特定用户的验证。

**问题**

能否将验证及其关联的批准下载到文件夹中？

**答案**

您可以访问和下载校样的打印摘要报告，该报告将包括所有版本的所有评论、回复、标记、操作和决策。

**问题**

当请求用户有权访问报告ProofHQ时，这也会授予他们访问左侧部分的权限(即 工作流、联系人、帐户设置等)？

**答案**

这将取决于其证明许可证级别。 如果管理员或Supervisor许可证对他们进行设置，他们将能够访问“联系人”，但无法访问“帐户设置”和“工作流”。 如果他们使用管理员许可证进行设置，他们将有权访问帐户设置和工作流。

**问题**

在我的组织中，项目经理向利益相关者发送审批请求以供审阅/评论。 您提到我们不应向批准字段添加名称，您如何作为项目经理将创意验证共享给利益相关者？

**答案**

“审批”字段用于文档审批，如果您只需要简单的文档审批，则可以使用此字段。 如果您需要验证审批（包含评论、标记和验证决定），则您需要将利益相关者添加到具有查看者和审批者验证角色的验证中。

**问题**

如何在已创建的任何验证中将人员添加为新角色？

**答案**

要添加验证收件人并在现有验证上选择他们的验证角色，您将需要遵循以下路径：在文档选项卡中选择验证>然后单击验证详细信息。 当验证详细信息窗口打开时，单击舞台右上角的省略号按钮并选择“共享”。 然后，您将能够添加收件人并选择他们的验证角色和电子邮件警报。

**问题**

如果我们向验证管理员/创建者授予对验证总部的访问权限，我们是否能够阻止管理区域，例如工作流、组等？

**答案**

是，这由用户验证权限决定。 具有经理或主管验证权限的用户无权访问帐户设置和工作流模板。 具有管理员验证权限的用户将有权访问帐户设置和工作流模板。 所有具有访问权限的用户都可以访问“组”区域。

**问题**

用户如何能够看到他们分配到的所有验证，而无需成为验证管理员？

**答案**

如果用户希望查看所有仍需要做出决策的验证，将可以使用Workfront中的“主页”或“我的更新”区域（具体取决于其访问级别）。 您还可以创建验证审批报告并应用过滤器，以仅显示登录用户是查看者和审批者的验证。

**问题**

您好，对于有3轮设计和反馈的情况，您是否可以回顾一下自动验证工作流，如何适应延迟提供反馈的情况，以及如何最好地将其绑定到WF中每一轮的任务中（设计和项目经理反馈）？

**答案**

您可以采用多种不同的方法，来利用任务以及审阅和批准。 我喜欢的方法是执行“验证路由”任务，并且我使用验证工作流管理发送给收件人的通知（而不是为他们分配任务）。 然后，您可以为“第2轮Proof路由选择”和“第3轮Proof路由选择”创建任务，这可以帮助您跟踪有多少轮进行了测试。 您还可以使用Proof功能板（ PHQ登录>功能板>要管理的验证）跟踪验证进度。 此视图将指示您正在管理的延迟验证（以及处于风险中的验证）的数量。

**问题**

删除验证时，该验证的副本是否仍保留在您的服务器上？

**答案**

可以。如果删除相关验证帐户的垃圾桶区域中的某个验证，则可以根据需要从该位置恢复，直到清空垃圾桶为止。

**问题**

如果另一用户拒绝或批准进行更改，是否可以触发新决策？ 即。 校对部门发现了一些内容，项目经理必须做出新决定……即使他们已查看并批准了该内容。 （尝试不让项目经理不必等待校对部门进行审阅）？

**答案**

虽然无法自动执行此操作，但您可以将项目管理器设置为决策电子邮件警报。 这样，当校对部门做出决定时，项目经理会收到所作决定的通知，然后可以返回校对，查看校对部门的意见，然后根据需要更改他们的决定。

**问题**

为什么当我在“验证”详细信息部分中发送更新时勾选“请求审批”时，我看到的只是SOC状态，而不是SOCD。 是否应避免使用此复选框？ 对验证发送更新的最佳实践是什么？

**答案**

使用“请求审批”功能时，您使用的是独立于校对和SOCD进度条的文档审批功能。 如果您需要更新验证收件人的验证角色，您需要执行以下路径：在文档选项卡中，选择验证> ，然后单击验证详细信息。 当验证详细信息窗口打开时，您将看到收件人列表，并且可以相应地调整验证角色（以及电子邮件警报）选项。 这允许您（例如）将验证角色从查看者更改为查看者和审批者。

**问题**

如果同一验证文档中存在早期版本（和注释），是否可以确保最终批准者无权访问这些版本（和注释）？ 是否需要创建新的验证文档，或者是否可以将所有版本和注释都保存在一个中，并指定对版本的访问权限？

**答案**

在验证内的帐户设置中，您可以控制对验证的共享/可见访问。 要更新此设置，以便验证收件人仅看到您指定的验证版本（而不是看到验证的所有版本），您需要遵循以下路径： PHQ登录>帐户设置>设置>共享>收件人可以查看所有版本=已禁用。

**问题**

能否将校样仪表板屏幕作为外部页面添加到WF仪表板？ 非管理员用户会看到仪表板吗？

**答案**

您可以将验证仪表板添加为仪表板中的外部页面。 请注意，这仅对拥有验证许可证的用户可见。

**问题**

ProofHQ中的仪表板和报告功能仅适用于有权访问Proof的管理员，对吗？ 不是没有管理员访问权限的常规规划人员？

**答案**

这是正确的。 但是，您可以向Workfront提交支持案例，以请求所有验证许可证用户都有权访问验证系统。

**问题**

您好，有关验证所有权灵活性的问题：如果在原始所有者不在的情况下需要上传新的验证版本，最佳实践是让他们在工作流中添加同事作为作者，然后他们会决定“不相关”？ （委派所有权似乎仅适用于单个版本）。

**答案**

此用例和工作流程将完全有效。 但是，您可以考虑的另一件事是，让可能需要上传新版本的用户来验证他们不是所有者，并使用主管或管理员的验证权限级别进行设置。 此权限级别将允许他们上传新版本来验证他们不是的所有者，而无需作为作者或审查方将它们添加到验证中（这都需要做出决定）。

**问题**

正如我所理解的，您不能在自动化工作流的后续阶段中添加相同的用户，这对我们来说是一个问题。 您是否可以对此进行更改以允许同一用户处于多个阶段？

**答案**

虽然您无法将验证收件人添加到验证的多个审核阶段，但是一旦激活审核阶段，他们将在该版本的剩余阶段中处于验证状态。 这将允许他们继续评论和回复评论，即使其他阶段已经开始。 确保此操作正常进行的关键是确保在启动新阶段时不会锁定阶段。

**问题**

能否说明阶段之间的验证路由？ 如何关闭一个并移到下一个阶段？

**答案**

在自动化工作流模板中，我们提供了一些选项，通过这些选项，可将从一个阶段移动到下一个阶段。 可使用的选项包括“创建验证时”、“当所有决策在父级阶段获得批准时”、“当所有决策在父级阶段获得批准或批准且有更改时”、“当所有决策在父级阶段中作出时”以及一些其他选项。

**问题**

是否可以从自动生成但不想作为验证的文档中删除验证？

**答案**

如果启用了“上载文档时自动生成验证”设置，您将无法从文档中删除验证。 相反，您将需要通过“新增”>“文档”按钮重新上传文档。

**问题**

用户在验证流程的阶段3发言能否添加另一个人作为审阅和批准者？

**答案**

如果该用户对验证具有编辑权限，则他们可以。 拥有编辑权限的用户将为：验证所有者、添加到验证的验证收件人和验证角色为作者或审查方、验证许可证用户及验证权限级别为主管或管理员的用户。

**问题**

如果用户被指定为作者，他们能否上传新版本的验证？ 这个人不是证据发起人。

**答案**

具有作者和审查方验证角色的验证收件人可以向该验证角色所属的验证添加新版本。

**问题**

外部用户会收到针对每个验证的电子邮件以供审阅。 这对于他们跟踪他们有效的所有验证的状态可能具有挑战性。 外部用户是否有任何功能板或电子邮件状态列表选项，或者即将推出的功能来跟踪其在多个验证中的状态？

**答案**

我建议将这些外部用户添加到具有免费查看者许可证的Workfront。 这将授予他们访问“我的更新”页面的权限，该页面将包含他们需要决策的所有未完成验证的列表。

**问题**

能否详细解释Decisions通知？ 我是将只收到包含审阅人和审批人校对注释的通知，还是将同时收到审阅人的注释以及何时会收到这些注释？

**答案**

仅当对验证做出决策时，才会发送决策电子邮件警报通知。 当有评论时，将不会发送它们。 但是，如果您收到决策电子邮件警报，表明验证上的收件人做出了需要更改的决定，那么您将知道现在正是查看他们添加的评论（这将在验证中）的好时机。

**问题**

关于转发电子邮件的问题，您实际是以电子邮件的所有者身份登录吗？ 在锁定的环境中会发生这种情况吗？ 在SSO环境中会发生这种情况吗？

**答案**

这会将您作为转发电子邮件给您的人员登录到验证中。 如果对验证使用“需要登录”并使用SSO，则将阻止您以电子邮件转发人的身份访问验证。

**问题**

在校对中，我该在何处访问仪表板和报告？

**答案**

如果您在Workfront中的搜索栏右侧有一个复选框图标，则表示您拥有集成的Workfront和验证帐户。 单击该复选框将会转到Workfront Proof，并且主屏幕将是功能板。 可以使用左侧面板中的视图选项构建报告。

**问题**

在“角色”部分下，底部有2个复选标记，提及将使用@mention等添加某人。 在“验证”设置中，您可以为每个人设置默认角色，但不能自动选中这些复选标记，因此每次创建验证时，您都必须选中。 如何使其成为用户的默认值？

**答案**

当前无法将此设置为验证收件人的默认设置。 但是，您可以在自动工作流模板中将这些设置另存为收件人的默认设置。

**问题**

如何切换验证所有者？

**答案**

要切换校对的所有者，您将要遵循以下路径：在文档选项卡中，选择校对并单击“校对详细信息”。 将打开验证详细信息选项卡。 如果要成为验证所有者的人员尚未出现在验证中，您将希望通过单击省略号按钮并选择共享来添加他们作为收件人。 将人员添加到验证后（或者如果他们已在验证中），您将选择其对应的“省略号”按钮以选择“成为所有者”。 现在他们将成为证明的所有者。

**问题**

对于新版本的验证……我了解的唯一方法是将文件拖放到现有文件上。 这是正确的做法吗？

**答案**

我建议通过此方式创建新版本：在文档选项卡中选择验证，然后单击更多按钮，选择新版本>验证。 此操作可将您转到新版本页面，该页面将会继续执行工作流，并且允许您在路由新版本之前进行任何所需的调整。

**问题**

能否禁用对验证的评论以便与客户共享，这样他们就不会看到团队的所有内部反馈？ 这样您就不必重新生成新的验证。

**答案**

我建议使用自动化工作流模板，这将允许您使用“专用阶段”。 专用阶段允许您隐藏其他阶段中来宾审阅人的注释、标记和决策。 这将允许外部请求者完全隐藏您的内部验证查看。

**问题**

Workfront Proof阶段是否仅在使用自动工作流且未添加到工作流的用户打开验证时添加？

**答案**

如果非收件人单击验证，则“Workfront Proof”阶段将被添加到验证中。 如果有人将基本工作流验证转换为自动Workfront Proof，也会应用该验证。

**问题**

我们是否能够设置一个验证工作流，以便做出多个决策？

我们努力向内部法律团队报告外部法律顾问何时完成审阅证明（他们平均需要多少天才能完成审阅、哪些人完成审阅等）

我们首先向验证工作流中添加了一个名为“OC审核完成”的新决策，并以为我们可以编写报告来跟踪这些决策。

问题是，似乎只能在工作流上做出一项决策。

**答案**

一个验证可以做出多个决策 — 但是，验证只有一个总体状态，该状态来自验证的最坏情况决策 — 或由主要决策者做出的决策。

由于您的报告要求，我建议您让验证中的每个人使用相同的决策选项（“已批准”、“已批准并更改”、“需要更改”），然后使用“验证仪表板”中的报告（“PHQ登录”>“报告”），并应用过滤器选项按收件人进行过滤（在过滤器中包含外部法律顾问收件人），随后您将能够查看其验证的平均周转时间。

**问题**

将新版本拖放到现有验证上后，为何所有角色都会更改或明确消失？

**答案**

将文档作为新版本拖放时，您从新版本中剥离工作流是正确的。 如果要保留上一个版本到下一个版本的工作流，请在“文档”选项卡中选择验证，然后单击“更多”按钮，选择“新版本”>“验证”。 此操作可将您转到新版本页面，该页面将会继续执行工作流，并且允许您在路由新版本之前进行任何所需的调整。

**问题**

情景 — 转发验证：查看验证的外部客户在批准我们的验证之前，可能希望在其组织内部分发。 其他审阅者不一定在系统中，因此评论中的@似乎不起作用。 他们应该如何最好地共享 — 转发电子邮件，然后向收件人突出显示任何评论都不会显示为他们的姓名？

**答案**

您需要使用校样订阅功能。 这可以在验证的设置中启用，并允许验证的收件人将通用公共链接转发到验证，然后允许用户订阅验证（实际上是添加自己）。

**问题**

在文档中使用文件夹的最佳实践是什么？

**答案**

这将取决于项目的性质，但有时可考虑为一个活动验证文件夹和一个批准验证文件夹，前者包含当前路由的所有验证/版本，后者包含最终批准和批准的所有验证。 完全审批验证后，将其从活动验证文件夹移入已审批验证文件夹。

**问题**

如果我有3个人参与审阅组，是否可以设置我需要这3人中的2人的审批？

**答案**

可以。您将需要两个人员作为审阅人和审批人来添加决策，第三个人员作为审阅人。

**问题**

我们希望向外部客户(非Workfront用户)发送验证以供其审核和评论。 我们希望向他们发送一个干净的证据（换言之，就是没有内部注释的证据）。 有哪些正确的步骤可实现这一点，以确保外部客户端获得验证（只有验证，无法访问项目本身），以及外部客户端如何“发送”我们备份其标记的验证？ 我们当前不使用验证模板/自动化工作流。

**答案**

我建议为此使用自动化工作流/自动化工作流模板，因为它将允许您使用“专用暂存”功能。 使用专用阶段功能时，您可以让评论/决策和审核特定阶段的收件人对其他阶段的人员保持隐藏。 例如，您可以将内部阶段作为专用阶段和客户端阶段。 客户端将无法看到与内部阶段有关的任何内容，而您能够看到客户端阶段中的活动。

**问题**

是否可以在一个早期阶段保留特定用户（又称校对器），而无需在后期阶段循环这些用户？

**答案**

将某人添加到某个阶段的验证版本后，其在剩余阶段中将保持在该版本的验证上。 您确实可以选择在下一阶段开始（或手动）时锁定其阶段，这将阻止他们再进行任何注释。

**问题**

在哪里可以查看已查看和/或批准验证的每个人的列表？哪一天？在什么时间？ 用于审核等 是否还有一处可查看所有验证版本的所有审阅和批准？

**答案**

要查看活动列表（如何时作出了评论和决策），您需要单击验证详细信息中的活动历史记录。 要访问此文档，请遵循以下路径：在文档选项卡中选择验证>单击验证详细信息>展开活动部分。 如果您想在版本级别查看此信息，请按照以下路径操作：在文档选项卡中选择验证>单击“详细信息”选项卡>朝向屏幕底部，您将看到版本部分。 在此处，您可以在版本级别访问验证详细信息。

**问题**

你能谈谈校对中的私密阶段吗？

**答案**

当阶段被设为私密时，未添加到此阶段或帐户中不是主管、管理员或账单管理员的用户看不到评论和决策。 此外，添加到专用阶段的审阅人只能看到他们被添加到验证中的阶段以及在该阶段所做的评论。
