# 开发者开源合规实践参考手册

## 0 关于本手册

本手册针对开发过程遇到的合规情况给出参考建议，开发者可根据自身开发情况借鉴此手册，尽量规避开源合规风险。

本文由Compliance sig组合作编写。

本手册内容依据 “CC-BY-SA-4.0” 许可证进行授权，详见CC-BY-SA-4.0。

## 1 README文件参考

开源软件通常都会提供Readme文件，用于说明项目基本信息，使用户快速了解上手该项目。绝大多数代码托管平台通常也将Readme文件内容默认展示在项目首页，可以说Readme文件就是开源项目的“脸面”。
一个优秀的Readme文件，其内容通常包含项目简介、安装构建步骤、帮助反馈等栏目。

- 项目简介一般包括项目背景、主要功能、同类软件对比等，部分优秀的项目也会提供设计架构、开发路线图等内容。
- 安装构建步骤提供软件包直接安装和源码编译构建安装的详细步骤，列出编译安装环境要求及关键配置等信息。
- 帮助反馈部分提供项目详细文档链接、常见问题解答及问题反馈方式等。

以上这些栏目内容通常无固定格式，由开发者自行编写。
除此之外，强烈建议开发者在Readme文件中声明本项目的版权及开源许可证（Copyright&License）信息。

a、 一般开源项目Readme文件声明版权及开源许可证（Copyright&License）参考模板如下：

```
##Copyright&License

Copyright（c）[time] [ name of copyright holder ]
[Project Name] is licensed under [LICENSE].Please check the LICENSE file for more information.

```

b、若为从其他开源项目衍生而来的项目，其Readme文件除上述声明内容之外还需声明上游开源项目相关信息，同时说明维护策略（例如独立发展或跟踪上游适配等策略）。示例如下：

```
[Project Name] is a fork of [Original open source software name]；
```
或
```
[Project Name] fork from [Original open source software name];
You can access the source open source software address through this URL：
                                  XXXX;
```

## 2 License声明参考

## 3 文件头版权信息编写参考

文件头版权信息一般包括copyright信息和LICENSE声明，其中copyright信息是一种软件作品署名权的体现方式，而LICENSE声明能够帮助使用者在使用时准确接收并继续传递该权属信息。

文件头版权信息原则上应该按照项目LICENSE文件中规定的格式编写。

a、部分LICENSE文件中会提供文件头版权信息格式，如项目LICENSE文件存在推荐格式，可直接按照LICENSE文件的格式编写，如下图为Mulan PSL v2 LICENSE文件提供的文件头版权信息格式：

```
Copyright (c) [Year] [name of copyright holder]
[Software Name] is licensed under Mulan PSL v2.
You can use this software according to the terms and conditions of the Mulan PSL v2. 
You may obtain a copy of Mulan PSL v2 at:
               http://license.coscl.org.cn/MulanPSL2 
THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.  
See the Mulan PSL v2 for more details.  
```

则版权信息为XXXX，时间为YYYY，许可证采用Mulan PSL v2 LICENSE的项目，文件头版权信息如下：

```
Copyright (c) XXXX  Co., Ltd. YYYY . All rights reserved.
XXX licensed under the Mulan PSL v2.
You can use this software according to the terms and conditions of the Mulan PSL v2.
You may obtain a copy of Mulan PSL v2 at:
     http://license.coscl.org.cn/MulanPSL2
THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
PURPOSE.
See the Mulan PSL v2 for more details.
```

采用其他LICENSE的项目可参考上述示例修改提供的格式。

b、 如项目LICENSE文件未提供推荐格式，可参考如下模板进行编写：

```
Copyright (c) [Year] [name of copyright holder]
[Software Name] is licensed under [Your LICENSE].
See LICENSE file for more details.  
```

如某项目版权信息为XXXX，时间为YYYY，许可证采用MIT LICENSE，文件头版权信息如下：


```
Copyright (c) XXXX Co., Ltd. YYYY. All rights reserved.
XXX is licensed under MIT LICENSE.
See LICENSE file for more details.  
```


c、 在开发过程中如需引用开源软件，则引用的开源软件文件头版权信息需完整保留，不得随意修改。如需对引用的开源软件进行修改，若修改的部分较少，可在修改文件文件头版权信息中添加修改声明，如该软件采用GPL-2.0或Apache系列LICENSE，则必须标注修改声明。修改声明格式示例如下： 

```
This file was modified by XXXX（Copyright owner）on YYYY（Time）
```


标注修改声明的文件文件头版权信息的格式示例如下：

```
Copyright (c) [Year] [name of copyright holder]
[Software Name] is licensed under [Your LICENSE].
See LICENSE file for more details.
This file was modified by XXXX（Copyright owner）on YYYY（Time）.
```

d、 若修改的篇幅较大或较有价值，需添加版权信息。

如新增代码文件，可参考上文添加版权头信息，注意LICENSE应与开源软件保持一致。

如新增较有价值的代码片段，可以注释的形式对该片段进行版权声明，参考格式如下：

```
***THE COPYRIGHT NOTICE START***
The copyright notice of this code snippet is as follows:
Copyright (c) XXXX（Copyright owner） Co., Ltd. YYYY. All rights reserved.
*******************************

……新增代码片段……

***THE COPYRIGHT NOTICE END***
```

## 4 Notice文件编写参考

## 5 License兼容性

## 6 spec文件License字段书写参考
spec文件中的License字段代表软件整体应遵守的开源许可证情况，为解决因许可证格式不统一引起的歧义(例如Apache-2.0，被简写为ASL-2.0、Apache-2、Apache License v2.0等)，应按照SPDX格式要求统一License字段书写格式。spec文件中License字段书写规范如下：
###  6.1、针对单一许可证

在确定好开源许可证的前提下，以SPDX的格式书写spec文件中的License字段，可通过[https://spdx.org/licenses/](https://spdx.org/licenses/。) 查找开源许可证的书写格式，现给出常见开源许可证的书写格式如下表所示：

| ***\*开源许可证完整名称\****                                          | ***\*SPDX格式标识符\**** |
| ------------------------------------------------------------ | -------------------- |
| BSD Zero Clause License                                      | 0BSD                 |
| GNU Affero General Public License v3.0 only                  | AGPL-3.0-only        |
| GNU Affero General Public License v3.0 or later              | AGPL-3.0-or-later    |
| Apache License 2.0                                           | Apache-2.0           |
| Artistic License 2.0                                         | Artistic-2.0         |
| BSD 1-Clause License                                         | BSD-1-Clause         |
| BSD 2-Clause "Simplified" License                            | BSD-2-Clause         |
| BSD 3-Clause "New" or "Revised" License                      | BSD-3-Clause         |
| BSD 4-Clause "Original" or "Old" License                     | BSD-4-Clause         |
| Creative Commons Attribution 4.0 International               | CC-BY-4.0            |
| Creative Commons Attribution Non Commercial 4.0 International | CC-BY-NC-4.0         |
| Creative Commons Attribution Non Commercial No Derivatives 4.0 International | CC-BY-NC-ND-4.0      |
| Creative Commons Attribution Non Commercial Share Alike 4.0 International | CC-BY-NC-SA-4.0      |
| Creative Commons Attribution No Derivatives 4.0 International | CC-BY-ND-4.0         |
| Creative Commons Attribution Share Alike 4.0 International   | CC-BY-SA-4.0         |
| Creative Commons Zero v1.0 Universal                         | CC0-1.0              |
| GNU General Public License v1.0 only               | GPL-1.0-only                  |
| GNU General Public License v1.0 or later           | GPL-1.0-or-later              |
| GNU General Public License v2.0 only               | GPL-2.0-only                  |
| GNU General Public License v2.0 or later           | GPL-2.0-or-later              |
| GNU General Public License v3.0 only               | GPL-3.0-only                  |
| GNU General Public License v3.0 or later           | GPL-3.0-or-later              |
| GNU Library General Public License v2 only         | LGPL-2.0-only                 |
| GNU Library General Public License v2 or later     | LGPL-2.0-or-later             |
| GNU Lesser General Public License v2.1 only        | LGPL-2.1-only                 |
| GNU Lesser General Public License v2.1 or later    | LGPL-2.1-or-later             |
| GNU Lesser General Public License v3.0 only        | LGPL-3.0-only                 |
| GNU Lesser General Public License v3.0 or later    | LGPL-3.0-or-later             |
| MIT License                                        | MIT                           |
| MIT No Attribution                                 | MIT-0                         |
| Mozilla Public License 2.0                         | MPL-2.0                       |
| Mozilla Public License 2.0 (no copyleft exception) | MPL-2.0-no-copyleft-exception |
| Mulan Permissive Software License, Version 1       | MulanPSL-1.0                  |
| Mulan Permissive Software License, Version 2       | MulanPSL-2.0                  |
| Do What The F*ck You Want To Public License        | WTFPL                         |
### 6.2、针对多许可证

spec文件中License字段应包含软件本身及引用的全部第三方开源组件（由依赖软件包或包管理器提供的除外）所涉及到的开源许可证，因此常见需要同时声明多个开源许可证。对于多许可证情况，除每个许可证均需采用SPDX格式相应标识符外，根据上游许可证约束要求，可使用AND、OR、WITH三种连接符进行组合。

(1) 当要求同时受多个开源许可证约束时，需使用AND连接符对许可证进行连接，参考示例如下：

License：Apache-2.0 AND MIT，表明该软件同时受Apache-2.0和MIT许可证约束。

(2) 当存在多个许可证，并且可由被许可人选择接受其中之一许可证进行约束时，需使用OR连接符对许可证进行连接，参考示例如下：

License：Apache-2.0 OR MIT，表明该软件可由被许可人选择受Apache-2.0或MIT其中之一许可证约束。

(3) 在现有许可证约束的条件下，被许可人希望获取额外权限时，需使用WITH连接符进行连接，参考示例如下：

License：GPL-3.0-only WITH Classpath-exception-2.0，表明该软件仅被GPL-3.0约束，被许可人还可选择Classpath-exception-2.0，从而获取额外权限。

### 附A 常见字符简介

spen文件License字段中会有一些字符经常与开源许可证组合使用，现对常见字符进行简介。

(1) 对于GNU许可证需使用only表明仅受GNU中的单一许可证约束。参考示例如下：

License: GPL-2.0-only，表明仅受GPL-2.0许可证约束。

(2) 单一许可证后加“+”字符，表明受单一许可证约束，也可由该单一许可证任何更高版本约束，由被许可方选择，参考示例如下：

License: EPL-1.0+，表明该软件受EPL 1.0或EPL许可证任何更高版本约束。

(3) 对于GNU许可证需使用later字符表示受GNU当前版本或更高版本的GNU许可证约束，由被许可方选择，参考示例如下：

License: GPL-2.0-or-later，表明该软件受GPL 2.0版本或更高版本的GPL许可证约束。

许可证组合及常见字符的详细介绍，可通过 https://spdx.dev/ids/ 进行参考。
