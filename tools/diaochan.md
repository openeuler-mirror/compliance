# 貂蝉

## 貂蝉网站简介
貂蝉是openEuler合规SIG组推出的开源合规SAAS服务的网站，目前已收录多个许可证及其元数据，并面向开发者提供API接口和开源项目的在线合规扫描服务。
网站地址为：https://compliance.openeuler.org/


## 功能介绍

### license查询
在网站首页输入license名称（支持模糊搜索），选择相应的license，会弹出其license信息。如下图所示，会显示其SPDX标准的license名称, 是否通过OSI（Source Initiative）或者FSF（Free Software Foundation）认可的license，以及license相应的权利、义务、限制等，还可以点击Full Text查看license全部内容。

![Apache-2.0信息查询](https://gitee.com/openeuler/compliance/tree/master/img/diaochan/apache-2.0.png)

### API使用
貂蝉网提供给开发者使用的API接口，可点击貂蝉网站右上角标签进入接口调用界面。

![进入API查询](https://gitee.com/openeuler/compliance/tree/master/img/diaochan/api.png)

开发者可以根据其licenseID值查询其license相关信息，licenseID可在貂蝉网站相应license的url上获取。如Apache-2.0 license链接为： https://compliance.openeuler.org/license/617 ，则其licenseID为617。
输入参数为其licenseID值，可查询相应licenseID相关信息。我们这里演示获取其license name，SPDX格式的名称，以及license的相关标签。
```
query {
  license(licenseID : 617) {
    id,
    name,
    spdxName,
    licenseMainTags {
      id,
      mainTag {
        id,
        type,
        name,
      }
    }
  }
}
```
点击界面中间的按钮，可显示其查询的标签信息。更多API特性及描述可参考右侧的docs。

![API调用](https://gitee.com/openeuler/compliance/tree/master/img/diaochan/api-use.png)

### 开源项目在线合规扫描
目前相关功能在开发完善中，合规扫描展示内容可能存在变化。

貂蝉网提供开源项目的合规扫描服务，目前展示的内容主要聚焦于开源项目的license和copyright风险问题。

点击右上角登录按钮：

![点击任务栏](https://gitee.com/openeuler/compliance/tree/master/img/diaochan/bookbar.png)

在弹出的界面中，点击授权按钮，目前支持gitee和github两种授权方式。

![授权界面](https://gitee.com/openeuler/compliance/tree/master/img/diaochan/login.png)

授权完成后，界面显示个人用户看板信息，浏览的历史报告信息、历史license信息都可以在这里查看。

在“我浏览过的报告”一栏，输入开源项目的仓库地址和分支，点击扫描。

![开源项目合规扫描](https://gitee.com/openeuler/compliance/tree/master/img/diaochan/how-to-scan.png)

扫描时间的长短与项目的大小、项目文件数量有关，等待一段时间，扫描完成。

![项目扫描中](https://gitee.com/openeuler/compliance/tree/master/img/diaochan/scan-process.png)

扫描完成后，点击Report ID即可查看扫描结果。
