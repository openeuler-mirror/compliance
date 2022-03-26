

# License合规问题(规则基线)

本规则旨在帮助社区开发者了解仓库中存在的合规问题，对于项目的合规而言，本规则是License合规的最低要求。License的合规问题包括但不限于此，下面列出的是一些常见的license合规问题。



| **问题**                          | **基线**                                                     | 说明                                                         |
| --------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1. 项目缺乏整体的License          | 在根目录（license、readme、copyright、notice等）或者1层子目录（/License(s)/License,  *Notice*/License等)下有文件中有License的完整文本的说明。 | 项目License文本内容应保证完整性                              |
| 2. 项目spec文件的License不规范    | License名称清晰性、规范性，不产生歧义                        | 项目的License名称不产生歧义，如License名称错误、未携带License版本号等 |
| 3. 缺乏项目级的Copyright声明      | 在根目录或者1层子目录，包括但不限于以下文件：License,  copyright, readme, notice 中的任何一个文件中包含copyrights字段描述 | 项目级的Copyright声明清晰性、规范性                          |
| 4.项目使用非FSF或OSI认证的License | 定义的可引入license合集                                      | 建议使用经过FSF或OSI认证的许可证，非认证许可证需经过评审     |
| 5. 第三方开源软件声明             | 若发布二进制文件，必须有第三方开源软件notice声明             | 建议原样保留第三方开源软件的License & Copyright              |



