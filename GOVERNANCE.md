# Compliance-SIG 治理公约

该Charter内容遵循openEuler [SIG-governance.md](https://gitee.com/openeuler/community/blob/master/en/technical-committee/governance/SIG-governance.md)描述的约定，本文会根据需要进行更新，以满足openEuler Compliance-SIG的需求。

为了使社区席位设置规范化和标准化，让社区参与者更好的融入社区,，Compliance-SIG 社区定义了两种角色：**maintainer**和**contributer**。



## 选举周期

Compliance-SIG 选举周期设置为当前新增maintainer当选时间到下一届maintainer换届选举时间，初步设置时间为每年的1月份和7月份。合规SIG组应定期审视项目贡献者和活跃度，每隔6个月进行maintainer的换届选举。所有的maintainer成员都需要参与换届选举，现有maintainer成员自动获得选举资格。在选举周期内，设置以下衡量指标：

## 贡献衡量指标

合规SIG对社区参与者的贡献做出了一系列衡量指标，衡量时间为当前选举周期，包括但不限于以下内容：

- 参与合规SIG例会或线下meetup次数6+
- 合规SIG例会或线下meetup分享次数2+
- 为项目编写教程、添加翻译、示例等文档类工作，教程、翻译、示例等文档必须内容完整独立并获得maintainer认可
- 参与commit信息审核、回答有关项目的问题（issue、PR等）、帮助社区闭环issue或者PR等累积次数3+，得到提问者认可
- 发现或提出合规工具、许可相关的bug、改进意见等累积次数4+（被社区接纳），相应的问题以issue的形式记录；或解决相应的bug、落地相应的意见累积次数2+
- 为社区做出技术贡献（如贡献新特性、技术方案、解决社区遗留问题等），并在openEuler社区落地
- 在合规SIG担任导师并带领参与者为合规SIG做出贡献
- 其它特殊贡献（需获得当前2/3 maintainer认可）

合规SIG仓库创建一个相应的贡献指标表格，用于统计相应的贡献指标，各参与者可自行提交PR到表格中，并由轮值maintainer完成合入。表格内容如下：

| 参与者 | 合规SIG例会参与次数 | 例会或线下meetup分享次数 | issue或PR闭环 | 发现或提出工具相关的bug、改进意见 | 教程、翻译等文档类工作 | 技术贡献 | 担任导师 | 其它特殊贡献 |
| ------ | ------------------- | ------------------------ | ------------- | --------------------------------- | ---------------------- | -------- | -------- | ------------ |
|        |                     |                          |               |                                   |                        |          |          |              |

对于贡献指标的衡量，若存在重复，重复指标不计算在内，如为项目编写教程，可能涉及PR、issue等指标。合规SIG遵从[openEuler社区行为准则](https://gitee.com/openeuler/community/blob/master/code-of-conduct.md)，若出现恶意刷指标、发布垃圾信息等行为，合规SIG可能采取的措施包括但不限于：

- 删除内容
- 屏蔽内容
- 将参与者拉入黑名单



## SIG **contributer**

### 成为contributer

contributer定义是长期活跃在社区的参与者。其社区行为符合上述定义的贡献指标两条或以上，或者获得当前maintainer一半以上的认可，但仅靠贡献并不能使贡献者成为maintainer。其还需要赢得当前maintainer和其他项目贡献者的信任，其决定和行动需要符合项目的最大利益。

### contributer权利

合规SIG组contributer有希望晋升成为maintainer，并可以影响maintainer选举投票。

- 合规SIG首页展示当前的contributer名单
- 获得社区活动、meetup等活动讲师资格
- maintainer候选人竞选投票权

## SIG maintainers

### 成为maintainer

- 符合上述定义的贡献指标四条及以上
- 获得当前maintainer提名
- 获得当前2/3的选举票

### Maintainer 权利

- openEuler社区合规SIG maintainer身份席位
- 合规SIG相关项目的选举、投票和提出议案的权利
- 负责批准PR是否可以合入
- 合规SIG 所有事务决策（除maintainer换届选举投票）都由maintainer共同投票决定，事务决策投票按照半数以上原则
- 指定遗留问题跟踪人
- 指导reviewer和其他贡献者
- 识别社区长期贡献者并对其maintainer候选人提名
- maintainer换届选举时，由现有maintain讨论决策增选maintainer人数，并共同参与公开投票

### Maintainer 义务

合规SIG按照[maintainer成员列表](https://gitee.com/openeuler/community/tree/master/sig/sig-compliance#maintainer%E5%88%97%E8%A1%A8) 的顺序进行轮值，轮值周期为当前主持合规SIG例会的时间到下一次召开合规SIG例会的时间，在轮值期间，主要负责这一段时间合规SIG的活动、运营工作等，并做好交接工作。maintainer成员的义务主要有：

- 参与合规SIG的双周例会次数不低于70%，例会时间冲突应委托他人参与
- 轮值主持双周例会


### 退出maintainers

Maintainer可以根据本人的自愿放弃请求或者在项目中无法有效履行maintainer职责而被移除权限。如果其决定退出maintainer队伍，轮值maintainer将建立PR将其从 OWNERS 文件中删除。 若maintainer未有效履行职责，在maintainer换届选举时，由轮值maintainer发起讨论，其他maintainer共同讨论决定是否移除maintainer候选人资格；若待讨论的maintainer恰好是轮值maintainer，则轮值maintainer由列表的下一位主持。

## 社区决策

openEuler 核心项目和SIG组都是具有开放设计理念的开源项目。这意味着代码仓是项目和SIG组理念、设计、发展规划等各个方面的真实来源。

因此，每个决定都可以表示为代码仓的更改。

所有影响Compliance-SIG代码仓的决策，无论大小，都遵循相同的步骤：

- **第 1 步**：建立PR或Issue。 任何人都可以做到这一点。
- **第 2 步**：讨论PR或Issue。 任何人都可以做到这一点。
- **第 3 步**：Maintainer合并、关闭或拒绝PR。

PR由 Compliance-SIG 代码仓的当前maintainer审查。



## 章程修改

sig-compliance的章程修改遵循openEuler [SIG管理指南](https://gitee.com/openeuler/community/blob/master/zh/technical-committee/governance/README.md#id2-2)，由maintainer代表提出修改意见，所有maintainer参与投票，获得2/3 maintainer同意方可修改。







