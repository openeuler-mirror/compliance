# 合规SIG组License准入审阅流程

1. **流程目标**: 识别一个新的License的与开源领域相关的风险情况。为openEuler的开源项目引入管理打下基础。根据识别的风险情况，制定不同场景下该License的准入情况。分为如下4种情况:
    1. “广泛认可开源的License” (FSF or OSI approved) >> 推荐使用 >> 可用做“自演进”项目（openeuler group下）的项目级License.
    2. “可使用”License >> 可使用 >> 可用做社区“开源使用”（依赖）的“组件”的License (src-openeuler group下也为该类）
    3. “受限使用”的License >> 限制使用（需备案）>> 备案，追踪该类License的使用情况，告知maintainer该类License的风险，Maintainer应寻求替换、隔离、限制使用场景等多种方式降低风险并自担责任。
    4. 禁止引入的的License, 不属于上诉3种情况的license.
2. **输入件 (流程发起资料表单）**：
    1. License ID ：如果该License在SPDX list 中，则使用SPDX identifier, 否则参考使用的最多的名字，定义一个ID
    2. License SPDX Identifier : 如果不在SPDX list中，则该项必须为空 
    3. License 别名：可以有多个
    4. License原文
    5. License原始出处: 该License原始出处的项目的网站（如有）和该License出处的描述 
    6. License是否被FSF或者OSI认可：FSF: <Yes|No>; OSI: <Yes|No>;
    7. License相近版本: 请给出该License FSF or OSI认证的相近的版本，并给出Diff(如有).
    8. License使用情况：请列明该License在其他Linux发行版中的认可度(必须覆盖Debian/Fedora/openSUSE)
    9. License影响范围：请给出该License影响哪些软件包源码仓库，并明确其二进制发布范围，当前有效范围包括Core/BaseOS/Everything/EPOL/Other
    10. License的涉及的负面的诉讼和争议情况：描述该类情况的文字(如有)。
3. **输出件**：
    1. 该License是否为openEuler approved的 “开源的” License.
    2. 该License 是否为openEuler 标记的”非开源需限制使用的“(简称：受限使用) 的License
    3. 如果以上都不是，则该License为“禁止”引入License.
4. **审阅原则**:
    1. 是否为openEuler approved 的“开源的”License: 
        1. FSF or OSI approved 的减去 是否为openEuler黑名单（很少）
        2. 如果该License有与其相近的License的是FSF 或OSI approved的，则可以对比两个License的差异部分，按照OSD的10条开源定义进行对比
    2. 是否为openEuler标记的“受限使用”License
        1. 不属于openEuler approved 的“开源的”
        2. 语言表述对分发、修改、使用等开源场景较为宽松
        3. 在开源领域被广泛使用
        4. 没有负面的诉讼和争议事件。
5. **审阅流程**：
    1. 申请人，按输入件要求，准备申请材料。
    2. 在合规SIG组双周例会上进行审阅
    3. 合规SIG组Maintainer按审阅原则进行投票，按参与投票Maintainer数量大于≥60%，赞成票≥60%，为通过某标记。
6. **结果发布和过程存档**：
    1. License标记列表：
        1. [https://compliance.openeuler.org](https://compliance.openeuler.org/) 页面上以表格形式发布
        2. 在openEluer compliance 仓库中管理该表格的yaml文件，通过提交记录了解其变更情况
    2. 审阅过程：
        1. 审阅申请资料和投票情况，通过合规SIG组会议纪要发出
        2. 审阅申请资料和投票情况，在compliance仓库中存档
7. **参考资料**:
    1. FSF查询站点：[https://www.gnu.org/licenses/license-list.html](https://www.gnu.org/licenses/license-list.html)
    2. OSI查询站点：[https://opensource.org/licenses](https://opensource.org/licenses/)
    3. Linux发行版License认可度查询站点：
        1. Debian: [https://wiki.debian.org/DFSGLicenses](https://wiki.debian.org/DFSGLicenses)
        2. Fedora: [https://docs.fedoraproject.org/en-US/legal/license-approval/#Software_License_List](https://docs.fedoraproject.org/en-US/legal/license-approval/#Software_License_List)
        3. openSUSE: [https://en.opensuse.org/openSUSE:Accepted_licences](https://en.opensuse.org/openSUSE:Accepted_licences)
