# compliance-sig会议信息

点击 ▶ 查看会议详情

## 2023

<details><summary>
20231216 openEuler Summit 2023 Call for SIG 开放工作组会议

*[etherpad 地址](https://etherpad.openeuler.org/p/20231216-summit-Compliance)*
</summary>

**\# 会议信息**

主题：openEuler-Compliance SIG开放工作组会议<br>
时间：2023年12月16日 16:00 - 18:00<br>
地点：国家会议中心4F主会场<br>
与会人：王悦良[@wangyueliang](https://gitee.com/wangyueliang)，许渊聪[@sectrend_xyc](https://gitee.com/sectrend_xyc)，丁紫薇[@dingziwei](https://gitee.com/dingziwei)，丁欣，程鑫鑫，郭怡如[@hana629](https://gitee.com/hana629)，陈一雄[@YixiongChen](https://gitee.com/YixiongChen)<br>

议程：
- 议题一：开源许可证案例知识库建设分享 by 许渊聪[@sectrend_xyc](https://gitee.com/sectrend_xyc)
- 议题二：操作系统软件包组件引用情况分析及治理边界讨论 by 王悦良[@wangyueliang](https://gitee.com/wangyueliang)

**\# 纪要内容**

**议题一：开源许可证案例知识库建设分享**

by 许渊聪[@sectrend_xyc](https://gitee.com/sectrend_xyc)

1. 开源许可证案例的知识库完成开发，包含欧拉社区许可证的评审依据记录、国外社区的开源许可证黑名单目录和国内外收录的许可证相关案例信息

2. 对存在合规案例的许可证进行了标签处理，便于检索许可证对应的案例进行分析

**议题二：操作系统软件包组件引用情况分析及治理边界讨论**

by 王悦良[@wangyueliang](https://gitee.com/wangyueliang)

1. 操作系统软件包成分复杂，包含软件源代码包、其他组件源代码包、vendor包、patch文件、spec打包文件、配置文件等，这些成分可能会从不同来源、以不同形式引入与目标打包软件版权和开源许可不同的成分，
这也为开源合规治理带来了更大的复杂度。
2. 其中spec文件中构建依赖涵盖静态链接库、编译接口/头文件、高级语言编译包，运行依赖涵盖动态链接库、高级语言运行时、运行环境、二进制可执行文件、高级语言运行依赖包等多复杂情况
3. patch文件涵盖自研、上游项目补丁回合、第三方补丁引入来源，针对其组件的片段引用、文件引用、组件引用复杂情况进行合规治理
4. 对于操作系统软件包复杂的成分，开源合规治理边界、以及面对合规治理与功能需求冲突时的平衡问题需具体探讨

</details>
 