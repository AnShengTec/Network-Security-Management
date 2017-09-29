# 物联网安全技术与管理
物联网是新一代信息技术的重要组成部分，也是“信息化”时代的重要发展阶段。
## 目录

1. 物联网及其系统架构
2. 物联网感知层的安全威胁及对策
3. 物联网网络层的安全威胁及对策
4. 物联网安全技术架构

## 一、物联网及其系统架构

*  物联网（Internet  of  Things）：是继计算机、
互联网与移动通信网之后的信息产业新方向，是
感知、互连、和智能的叠加

*  物联网应具备以下三方面能力：
   * 全面感知：RFID、传感器等随时随地获取物体信息
   * 可靠传递：通过各种网络融合、业务融合、终端融
合，准确传输物体信息和反馈信息
   * 智能处理：利用云计算、模糊识别等各种智能计算
技术，对海量数据进行分析和处理，对物体进行智能
化控制。

物联网系统架构：公认的三层架构 

 ![](/image/image_matter_01.jpeg)


### 1.1 物联网及其系统架构-感知层

* 感知层主要功能
 *  解决人类世界和物理世界的数据获取问题
 *  包括数据采集和数据短距离传输两部分
 
 
*  实例：躯感网
    *   Body  Sensor  Network 
* 感知层主要技术

 * 传感器技术
 * RFID技术
 * 二维码技术
 * 短距离无线通信技术（ZigBee、蓝牙） 

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_02.jpeg)

### 1.2 物联网及其系统架构-网络层

*    网络层主要功能

 * 主要解决感知层所获取数据的远距离传输

 * 传输无障碍、高可靠性、高安全性

 * 物联网网络层将承担比现有网络更大的数据量和面
临更高的服务质量要求 

*    网络层主要技术

 * Internet  IPv6技术
 * 移动通信网（4G/5G、WiFi、WiMAX）
 * 无线传感器网络
 * 异构网融合技术 
 

*    应用层主要功能

 * 信息处理，决策管理（应用程序）
 * 人机界面（终端设备） 

*    应用层主要技术

 * M2M技术
 * 云计算
 * 人工智能
 * 数据挖掘
 * 中间件 

物联网安全问题分层模型

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_03.jpeg)


##  二、物联网感知层的安全威胁及对策

*    感知层安全威胁

 * 终端破坏与窃取
 * 节点仿冒与入侵
 * 传输信息窃取与侦听
 * 路由干扰
 * 拒绝报务 
 
*    感知层安全威胁对策

 * 密钥技术
 * 安全路由协议
 * 攻击检测 

### 物联网感知层安全对策(示例)

*  用户身份识别：生物识别技术

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_04.jpeg)

*  动态节点身份识别

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_05.jpeg)

*  植入式生物传感器安全对策

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_06.jpeg)


## 三、物联网网络层的安全威胁及对策

*  无线网络安全
 * 问题：监听、攥改、未授权信息服务、无线干扰等
 * 对策：身份认证、数据加密、消息完整性验证、密
钥管理


*  Pv6安全机制及问题
 * IPSec
 * 扫描与探测，邻居发现协议等新问题


*  异构融合安全问题 
*  海量数据处理和业务控制策略的安全性和可靠性
*  云平台安全访问控制
*  中间件安全控制
*  用户隐私数据保护 


### 数据安全解决方案（示例）

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_07.jpeg)

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_08.jpeg)

![](https://github.com/AnShengTec/Network-Security-Management/blob/master/image/image_matter_09.jpeg)

## 四、物联网安全技术架构

* 基础核心技术：
    * 密码技术
    * 高速密码芯片
    * PKI公钥
    * 基础设施
    * 信息系统平台安全等


* 防御关键技术：
    * 攻击检测
    * 内容分析
    * 病毒防治
    * 访问控制
    * 应急反应


* 网络环境安全技术：
    * 安全路由
    * 防火墙
    * 安全域策略
    * 无线网络安全
    * 安全审计


* 应用环境安全技术：
    * 可信终端
    * 身份认证
    * 访问控制
    * 安全审计

&copy; 2017，Ricky
