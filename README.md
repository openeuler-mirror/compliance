# Compliance

开源软件的使用已经渗透到多种行业，针对开源软件开发、使用的合规问题也越发得到重视。根据开源软件的生命周期和使用范围，将开源合规分为**license & Ｃopyright 合规 、 专利合规 、 出口管制合规 、 GDPR 合规 、 商业秘密合规 、 商标合规**等。本小组专注于合规相关领域的研究，将研究结果通过意见、工具等形式提供给社区进行开源合规管理的支持。

---

### Compliance 背景介绍
openEuler 作为操作系统开源社区，本身使用是的木兰 V2 版本协议，下游多家商业公司基于 openEuler 制作了商业发行版。openEuler 操作系统集成了上游开源社区数万个开源项目，这些项目使用了各种 License 。openEuler 使用的木兰 V2 协议和这些上游项目使用的开源协议之间是否存在不兼容情况，这些上游项目是本身是否存在协议不兼容的问题，需要有一系列的规则和工具来解决。譬如：

- 解决文件级license的问题。例如：PHP
- 解决新引入组件的license的判断问题。
- 解决上游组件license变更的问题。例如：mangoDB、ES
- 解决RPM包的spec文件license和原生社区的license不一致的问题。例如：greenlet组件

---

### license & Ｃopyright 合规
一般公众都认为开源代码是可以“免费”使用的，但这里的”免费“并不意味着可以随心所欲，而是要遵循License的约束，那么
- 到底License是什么？
- 开源代码的作者又为什么有权力指定License，进而对使用者进行约束呢？
- 开源领域的License和Copyright全规具体包含哪些方面呢？

本章节将尝试为大家一一解释：
1. [理解Copyright和License的本质](https://gitee.com/openeuler/compliance/blob/master/guideline/Concept.md)
2. [License和Copyright合规](https://gitee.com/openeuler/compliance/blob/master/guideline/license.md)
3. [FAQ](https://gitee.com/openeuler/compliance/blob/master/guideline/faq.md)
4. [术语与缩略语](https://gitee.com/openeuler/compliance/blob/master/guideline/terms.md)

---

### 出口管制合规介绍
我们希望通过该SIG制定满足社区的规则，并将规则build-in到流程中，通过工具和工程方法落地这些规则，最后可以提供解决方案或服务给参与社区的组织和个人。

#### 目标
1、梳理业务问题
2、洞察业界标杆社区、标准、规则、形成方法论
3、发布license相关规则
4、设计业务架构
5、设计软件架构
6、软件开发

#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request


#### 特技

1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
