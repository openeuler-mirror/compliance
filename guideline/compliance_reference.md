# 开发者开源合规实践参考手册

## 0 关于本手册

本手册针对开发过程遇到的合规情况给出参考建议，开发者可根据自身开发情况借鉴此手册，尽量规避开源合规风险。

本文由Compliance sig组合作编写。

本手册内容依据 “CC-BY-SA-4.0” 许可证进行授权，详见CC-BY-SA-4.0。

## 1 README文件参考

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
