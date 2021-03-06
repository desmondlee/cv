---
layout: cv
title: 李振国的简历
email:
  url: mailto:13816981250@139.com
  text: 13816981250@139.com
homepage:
  url: https://wp.lizhenguo.cn
  text: https://wp.lizhenguo.cn
---

# 李振国 **简历**

<!--
include contact information from the front matter
Supported arguments:
    - homepage: url, text
    - phone
    - email
-->

{% include cv-contact.html %}


## 个人信息
**生日：**1989.06; **籍贯：**江苏; **学历：**全日制本科; **工作经验:**6年开发

## 教育背景

### **常熟理工学院** `2009.09 - 2013.06`

```
软件工程，本科
```

- 软件工程学士学位
- 英语六级

## 技能标签

**Laravel**, **Yii2**,  Linux, Nginx, Mysql, Php(LNMP), Redis, Python, Go, jquery, css+div

## 自我评价
1. 做事认真负责，热爱工作，善于团队沟通；
2. 能承担压力，勤于思考，勇于迎接新挑战，善于分析与解决问题。

## 工作经历

### **1）上海基分文化（趣头条）**   `2020.04 - 2020.08` 

```
PHP工程师
```
<br>
_主要负责公司的信息化建设：OA系统、招聘系统、绩效系统等。_
<br>

<br>
主要工作内容：<br>

**项目一：OA系统**<br>
1. 借助**流程引擎activiti**，实现流程审批，如费用报销、对公支付等；
2. 打通金蝶系统，使费用报销部分能在金蝶系统实时生成凭证，降低金蝶维护成本。

<br>

---


**项目二：招聘系统**<br>

1. 实现了多简历版本的升级转换，使面试安排更加丰富多样(一个人可以有多份简历，参与多份职位的面试安排)；
2. 使用redis队列、supervisord等服务，优化流程处理逻辑，使主流程执行快速高效，同时又能**异步实时**处理相关事务(如企业微信消息通知、邮箱推送、日志记录等)。
3. 引入libreoffice等服务，实现简历格式转换，提升使用体验(如doc转pdf)。

<br>

---


**项目三：绩效系统:**<br>

1. 实现并完善Peers评价部分，提升系统可用性。

<br>

---


**项目四：其他内容:**<br>

1. 接入**配置中心**，实现敏感信息集中管理；
2. **维护centos服务器**，搭建supervisord, libreoffice等服务，为项目引入提升性能的服务；
3. 初步实现Docker容器化(目前仅测试环境)，实现资源优化，节约服务器成本；

**成就·证书**<br>
1. 最佳新人证书
2. 最佳项目证书
3. 容器学习认证证书
4. 优秀绩效

**离职原因**<br>
公司经营不善，大量裁员

### **2）浅橙网络科技**   `2016.10 - 2019.12` 

```
PHP工程师
```

<br>
主要工作内容：<br>

**项目一：信用卡/APP推广系统（PHP， Laravel）:**<br>
简介：<br>
多层级分佣型产品推广平台，通过发展团队及下线，引导用户下单办卡来获取佣金。

主要功能模块：<br>
产品管理，订单管理，团队管理，钱包管理，活动管理等。

**本人主要负责部分：**<br>
产品管理，订单管理，佣金结算等后台管理功能及对应API。

**负责部分功能特点：**<br>
产品管理部分支持多标签、多权重，智能排序等；<br>
订单管理部分支持前置、后置订单类型；<br>
结算部分支持在线查询结算、线下脱敏数据上传结算等方式以及多层级分佣。<br>


**用到的技能特点：**<br>
1. 使用redis做部分数据缓存，提高查询速度，如产品详情，用户信息等。<br>
2. 使用predis扩展做延时队列，异步处理消息发送等耗时服务，如短信通知、微信模板通知等。<br>
3. 各服务间通过event事件实现多关联、松耦合，如下订单时，会有消息中心，活动中心等订阅并处理该事件。<br>
4. 使用horizon可视化监控队列消耗等情况，及时发现并处理性能瓶颈。
5. 使用ELK做日志收集查看，及时发现重要业务日志或错误日志。

---

**项目二：信用卡进度查询服务（Python， mosquitto）**
简介：<br>
通过封装统一的查询界面，适配多家信用卡进度查询。
<br>

主要功能特点：<br>
1. 手机端通过websocket实现与mosquitto服务间的通信；<br>
2. python爬虫负责模拟用户操作与银行服务交互，并返回银行结果信息；<br>

<br>

**本人主要负责部分：**<br>
实现多家银行的信用卡的python查询服务。

<br>

**用到的技能特点：**<br>

1. 使用selenium模拟用户点击、输入等操作。
2. 使用Image库的crop函数从screenshot截图中截取验证码，防止验证码过期。


---

**项目三：贷后催收管理系统（PHP， Yii2）**<br>

简介：<br>
面向数千催收员的，为金融贷款公司提供催收服务的管理平台。<br>
<br>

主要功能模块：<br>
开放平台API，催收机构/人员管理，逾期订单管理，催收数据统计，逾期订单管理等。<br>
<br>

**本人主要负责部分：**<br>
多数都有参与，参与了多个功能模块从无到有的开发。<br>

<br>
主要功能特点：<br>
每天批量派单数十万单逾期订单；订单逾期状态实时更新；多种统计数据定时更新；对接多种SAAS服务；<br>
提供催收系统对外API，为多家金融公司提供催收平台服务。<br>
<br>
用到的技能特点：<br>
1. 数据库采用分表方式存储上亿催收记录信息。
2. 采用ID分隔方式，多进程派单。
3. 设计开放平台API时，采用先落库后处理的方式，实现第三方数据及时存储、延时更新。


### **3）国兆电子科技**   `2013.12 - 2016.10` 

```
PHP研发经理
```

<br>
主要负责以下系统相关功能开发：<br>

**项目一：微信公众号管理系统**<br>
简介：<br>
实现多公众号管理，应用功能模块化开发。
<br>
主要功能模块：<br>
粉丝管理，应用模块管理，素材管理等。
<br>

**本人主要负责部分：**<br>
参与并主导应用模块的需求确认、设计及开发。
<br>
用到的技能特点：<br>
1. 通过设定规范的路由规则，实现应用模块化加载。
2. 使用redis做数据缓存，使用数据库做延时处理。


---

**项目二：汽车融资租赁系统**
简介：<br>
提供web端查询二手车可融资贷款估价服务平台。
<br>

**本人主要负责部分：**<br>
全部由本人设计并开发。 
<br>

用到的技能特点：<br>
1. 使用JQueryMobile，JQuery制作web界面。
2. 使用PHP制作爬虫，定期更新系统中相关车型在汽车之家上的价格。



<!-- ### Footer

Last updated: May 2013 -->
