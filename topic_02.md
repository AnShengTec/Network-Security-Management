# 边界网络安全风险分析攻击手段识别

## 目录
1. 资产管理
2. 风险分析
3. 数据监控


## 一、资产管理

![](/image/image_safety_01.jpeg)

核心资产

* 企业：数据库、代码、敏感文件
* 员工：邮件、OA、CRM、员工权限
* 用户：资金、账户、个人信息

##### 核心资产受到威胁的后果：

雅虎5亿数据泄露后

![](/image/image_safety_02.jpeg)

CSDN用户数据库泄露

![](/image/image_safety_03.jpeg)

艾滋病患者信息泄露

![](/image/image_safety_04.jpeg)

攻击过程

![](/image/image_safety_05.jpeg)


攻击思路

![](/image/image_safety_06.jpeg)




## 二、风险分析


入侵过程：

*  外部信息收集->突破边界->内网信息收集->权限延伸&提升->数据获取

边界资产：

* 1）终端：PC、手机
* 2）设备：路由器、摄像头
* 3）应用：业务服务（web应用）
* 4）人员：员工

### 运维漏洞：

*  服务弱口令：SSH、RDP、Telent、VNC、各类数据...
*  代码泄露：SVN、Git、自建gitlab...
*  第三方组件升级不及时：Structs2、Java反序列化、CMS


#### 运维漏洞举例：


网站备份泄露

![](/image/image_safety_07.jpeg)

业务无关代码未及时删除-JS泄露敏感信息

![](/image/image_safety_08.jpeg)


测试账号未删除
```javascript
  <?php
  /*测试账号 */
  /*499719424   123456789 */
  /*195304023   Abc123456 */
  /*332012899   Abc123456 */
  define("USERNAME",""); //QQ账号
  define("PASSWORD",""); //QQ密码
  define("REPLAY","parse.ini"); //相关回复解析
```
备份文件

![](/image/image_safety_09.jpeg)

配置文件未及时删除

![](/image/image_safety_10.jpeg)


### 应用漏洞

* web 应用漏洞：Sql注入攻击、XSS攻击

### Sql注入危害

  * 窃取数据库敏感信息
  * 对数据进行恶意增删改
  * 造成拒绝服务攻击
  * 获取服务权限
  
例：
```javascript
“select * from product where id =”. $_GET[‘id’]
“select * from person_info where username=‘”.$_GET[‘name’].“’”
```

### RCE远程代码执行

![](/image/image_safety_11.jpeg)


###  风险分析
合理的资产管理->梳理攻击面->寻找脆落点->安全防护办法



## 三、数据监控

被动防御的劣势越来越明显

Struts2 应用漏洞
WannaCry 蠕虫传播

大数据分析平台

* 网络设备日志
* 安全设备日志

#### 理想状态

通过异常发现所有“所有攻击”：Web攻击、钓鱼软件、木马病毒等

#### 现实情况

无法覆盖100%的场景

#### 安全体系架构

![](/image/image_safety_12.jpeg)



&copy; 2017，Ricky