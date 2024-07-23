# openEuler社区代码仓License风险类别处理

### 说明：社区代码仓库License风险主要分为以下几类：

<table>
  <tr>
    <td><strong>License检查结果</td>
    <td><strong>风险类别</td>
    <td><strong>处理方法</td>
  </tr>
  <tr>
    <td rowspan='3'>not_allow</td>
    <td>低风险（受限使用），具体查看准入清单中<font color='red'>lowRisk</font>为<font color='red'>Y</font>的License</td>
    <td>检查、确认License使用范围</td>
  </tr>
  <tr>
    <td>禁止使用，具体查看准入清单中<font color='red'>black</font>为<font color='red'>Y</font>的License</td>
    <td>禁止引入使用该License仓，如有疑问咨询合规SIG</td>
  </tr>
  <tr>
    <td>未审阅，具体查看准入清单中<font color='red'>review</font>为<font color='red'>N</font>的License</td>
    <td>在合规SIG仓下提交License审阅申请issue，参考审阅流程：<a href="https://gitee.com/openeuler/compliance/blob/master/doc/rule/合规SIG组License准入审阅流程.md"> License准入审阅流程</a></td>
  </tr>
  <tr>
    <td rowspan='3'>unknow</td>
    <td>缺少版本、语法错误、非法链接符、非业界常见写法，具体查看准入清单中<font color='red'>alias</font>与<font color='red'>identifier</font>的写法</td>
    <td>代码仓责任人解压源码包、查看具体License声明并修正</td>
  </tr>
  <tr>
    <td>非License写法</td>
    <td>代码仓责任人解压源码包、查看具体License声明并修正</td>
  </tr>
  <tr>
    <td>不存在于准入清单中的新License</td>
    <td>代码仓责任人解压源码包、查看License声明信息，并在合规SIG仓下提交License审阅申请issue，参考审阅流程：<a href="https://gitee.com/openeuler/compliance/blob/master/doc/rule/合规SIG组License准入审阅流程.md"> License准入审阅流程</a></td>
  </tr>
</table>

---
#### License准入清单：https://gitee.com/openeuler/compliance/blob/master/doc/rule/Licenses_Access_List.yaml

#### 如有问题咨询合规SIG组：https://gitee.com/openeuler/compliance
