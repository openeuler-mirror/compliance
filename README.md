# compliance

当今随着开源软件使用越来越多，大家对合规的要求也越来越高。合规分为license合规、copyright合规、专利合规、出口管制合规、GDPR合规、商业秘密合规、商标合规等。

#### License compliance背景和困难
openEuler集成依赖了上游数千个开源组件，组件和组件之间也存在着复杂的依赖关系，RPM包的管理机制也带来了license合规的一些困难，目前我们看到的主要有以下几种情况：

- 这些组件的license不能覆盖其下的文件时，需要对文件级的license，大大增加了管理的难度；例如：PHP
- openEuler的Mulan 2.0的license是否和其依赖的开源软件兼容；直接依赖的软件和间接依赖的软件之间是否兼容，需要人工判断，工作量巨大；例如：木兰和ApacheV2.0、木兰和GPLV2.0、GPLV2.0和MIT等
- 新引入组件的license有哪些风险是需要注意的；例如：copyleft的license
- 上游社区依赖软件新的版本license变更后怎么办？例如：mangoDB、ES
- RPM包的spec文件license和原生社区的license不一致的时候怎么办？例如：greenlet组件

#### copyright合规介绍

#### 出口管制合规介绍


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
