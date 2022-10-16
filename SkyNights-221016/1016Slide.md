---
marp: true
theme: gaia
footer: '柳迪潇 2022-10-16'
paginate: true
style: |
  section {
      font-size: 35px;
  }
---

<!--
_class: lead gaia
_paginate: false
-->
# **企业级计算机硬件杂谈**
### 柳迪潇

</br></br>

---
## "服务器" ("Server")

啥是服务器？

TOP500 June 2022 #1
**FRONTIER**

Core(s): 8,730,112
Rmax: 1,102 PFlop/s

https://www.olcf.ornl.gov/frontier/

![bg right h:12cm](https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Frontier_Supercomputer_%281%29.jpg/2560px-Frontier_Supercomputer_%281%29.jpg)

---
## "服务器" ("Server")

啥是服务器？

**Dell R730**

"Skynet" Network Infra

![bg right h:11cm](https://i.dell.com/is/image/DellContent/content/dam/ss2/product-images/dell-enterprise-products/enterprise-systems/poweredge/poweredge-r730/pdp/server-poweredge-r730-pdp-ng-hero-static-v2.jpg?hei=402&qlt=90,0&op_usm=1.75,0.3,2,0&resMode=sharp&pscan=auto&fmt=pjpg)

---
## "服务器" ("Server")

啥是服务器？

**❤ Home ❤ Made ❤**
Supermicro H11 DSi
Epyc 7402

ESXi Server

![bg right h:9cm](image/supermicro.jpg)

---
## "服务器" ("Server")

啥是服务器？

**RockPi S**
3D Printer on Air
TCP-Serial

![bg right h:8cm](image/rockpi.jpg)

---
## "服务器" ("Server")

啥是服务器？

**Raspberry Pi Zero W**
Lights on/off

Core(s):
Rmax: 0.247 GFlop/s

https://web.eece.maine.edu/~vweaver/group/green_machines.html

![bg right h:4cm](image/pi0.jpg)

---

### "企业级"

<br></br>

- 免工具维护
* 冗余设计
- 热插拔

![bg right w:16cm](https://pic1.zhimg.com/v2-d6c1f3fdf33bdae4f5387561af7398a5_720w.jpg)

---

### "起夜级"

![bg h:12cm](image/potato.jfif)

---

## 物理结构

### 分类

</br>

- 机架式(Rack)
* 塔式(Tower)
- 刀片式(Blade)

![bg right w:16cm](https://www.racksolutions.com/news//app/uploads/Rack-server-and-blade-server-together.jpg)

---
#### 机架式(Rack)

![w:16cm](https://i.dell.com/is/image/DellContent/content/dam/ss2/product-images/dell-enterprise-products/enterprise-systems/poweredge/poweredge-r730/pdp/server-poweredge-r730-pdp-ng-hero-static-v2.jpg?hei=402&qlt=90,0&op_usm=1.75,0.3,2,0&resMode=sharp&pscan=auto&fmt=pjpg)

![bg right w:16cm](https://i.dell.com/das/xa.ashx/global-site-design%20WEB/92612f85-41af-5daf-b5d7-030f7bf68796/1/OriginalJPG?id=Dell%2fProduct_Images%2fDell_Enterprise_Products%2fEnterprise_Systems%2fPowerEdge%2fPoweredge_R730%2fpdp%2fserver-poweredge-r730-pdp-love-02.jpg&qlt=100%2c0)

---
#### 塔式(Tower)

![bg w:16cm](https://i.dell.com/is/image/DellContent//content/dam/ss2/product-images/dell-client-products/peripherals/dellemc_pet640_16x25_bezel_lf.psd?fmt=png-alpha&pscan=auto&scl=1&hei=402&wid=402&qlt=100,1&resMode=sharp2&size=402,402&chrss=full)

![bg w:8cm](https://i.dell.com/is/image/DellContent//content/dam/images/products/servers/poweredge/t640/dellemc-pet640-16x25-b.psd?fmt=png-alpha&pscan=auto&scl=1&hei=402&wid=240&qlt=100,1&resMode=sharp2&size=240,402&chrss=full)

---

#### 刀片式(Blade)

![bg w:12cm](https://i.ebayimg.com/images/g/FkYAAOxyGxxSKdTM/s-l500.jpg)

![bg w:15cm](https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/IBM_HS20_blade_server.jpg/1920px-IBM_HS20_blade_server.jpg)

---
## 以 R730 为例

</br></br>

#### $\quad$ 风道设计 (Cover)



![bg right w:18cm](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20003038.png)

---
## 以 R730 为例

![bg w:15cm](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20003249.png)

![bg w:15cm](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20003304.png)

---
## 组成单元

- 主板 (Motherboard)

* 中央处理器 (CPU)

#### Difference between server and PC CPU

* 频率较低-单核弱
* 核数高、缓存大-多核强
* 总线吞吐速率大

---
##### Intel

![bg h:13cm](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20005952.png)

![bg h:13cm](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20010157.png)

---
##### AMD

![bg w:16cm](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20005912.png)

![bg w:15cm](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20010106.png)

---
### 内存 (Memory)
</br></br>


##### Thx rxgg @王若溪!!!!
---
![bg](./image/内存_01.png)

---
![bg](./image/内存_02.png)

---
![bg](./image/内存_03.png)

---
![bg](./image/内存_04.png)

---
![bg](./image/内存_05.png)

---
![bg](./image/内存_06.png)

---
![bg](./image/内存_07.png)

---
![bg](./image/内存_08.png)

---
![bg](./image/内存_09.png)

---
![bg](./image/内存_10.png)

---
![bg](./image/内存_11.png)

---
### 电源 (Power Supply Unit, PSU)

![](https://snpi.dell.com/snp/images/products/large/en-us~750-ABBQ/750-ABBQ.jpg)

---
### 存储

#### SAS (Serial Attached SCSI)

接口向下兼容 SATA (Serial AT Attachment, Serial ATA)

![SATA and SAS](https://demartek.principledtechnologies.com/Images/SAS_SATA_Connectors.png)

---
##### Physica interface

![bg w:15cm](https://demartek.principledtechnologies.com/images/Mini_SAS_HD_compare-1.png)

![bg w:15cm](https://demartek.principledtechnologies.com/images/Mini_SAS_HD_compare-2.png)

---
#### SAS与SATA接口带宽比较
</br></br>

* SAS: 3 Gb/s in 2005, 6 Gb/s in 2009, 12 Gb/s in 2H 2013

- SATA: 1.5 Gb/s in 2003, 3 Gb/s in 2005, 6 Gb/s in 2010 (traditional SATA is not expected to extend beyond 6 Gb/s)

---
#### 为什么SAS更适合应用在服务器和工作站上

* 读写速度
- 价格
* 智能技术
- 外围硬件生态

---

##### jmicron 七宗罪

他家的usb sata，pcie sata，sata raid控制器，sata port multiplexer只做到了“能用”的水平，但是价格低所以大家用的硬盘盒、易驱线里面基本都是这些

##### Bug 大赏

![w:30cm](image/sata_problems.png)

[Multiply your problems with SATA Port Multipliers and cheap SATA controllers | TrueNAS Community](https://www.truenas.com/community/threads/multiply-your-problems-with-sata-port-multipliers-and-cheap-sata-controllers.96631/)

---
#### RAID
##### RAID controllers

![bg h:13cm](https://snpi.dell.com/snp/images/products/large/en-us~490-BDUT/490-BDUT.jpg)

---
#### SAS expanders
![w:19cm](https://t7m8e9c8.rocketcdn.me/wp-content/uploads/2020/02/raid-sas.jpg)

---
#### M.2, U.2 & NVMe

##### M.2
![bg h:16cm](https://ae01.alicdn.com/kf/H4ee7687701024be3899244d0a57ed1dfN/M-2-SSD-to-U-2-Adapter-2in1-M-2-NVMe-and-SATA-Bus-NGFF-SSD.jpg)

---
#### M.2, U.2 & NVMe
##### U.2

![bg h:12cm](https://demartek.principledtechnologies.com/Images/Demartek_SFF-8639.png)

---
#### M.2, U.2 & NVMe
##### NVMe (Non-Volatile Memory Express)

![bg h:9cm](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Intel_P3608_NVMe_flash_SSD%2C_PCI-E_add-in_card.jpg/450px-Intel_P3608_NVMe_flash_SSD%2C_PCI-E_add-in_card.jpg)
![bg h:9cm](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Ssd_960.jpg/450px-Ssd_960.jpg)

---
#### 智能平台管理接口 (Intelligent Platform Management Interface, IPMI)

原本是一种Intel架构的企业系统的周边设备所采用的一种工业标准。
* 1998年Intel、DELL、HP及NEC共同提出IPMI规格，可以透过网络远程控制温度、电压。

* 2001年IPMI从1.0更新至1.5，新增PCI Management Bus等功能。

* 2004年Intel发表了IPMI 2.0的规格，能够向下兼容IPMI 1.0及1.5的规格。新增了Console Redirection，并可以通过Port、Modem以及Lan远程管理服务器，并加强了安全、VLAN 和刀片服务器的支持性。

---
#### 特性
</br>

* IPMI独立于操作系统外自行运作，并容许管理者即使在缺少操作系统或系统管理软件、或受监控的系统关机但有接电源的情况下仍能远程管理系统。IPMI也能在操作系统启动后活动，与系统管理功能一并使用时还能提供加强功能，IPMI只定义架构和接口格式成为标准，详细实现可能会有所差异。

---
#### 组成
![bg right h:10cm](https://upload.wikimedia.org/wikipedia/commons/f/f2/IPMI-Block-Diagram.png)


* IPMI包含了一个以基板管理控制器(BMC)为主的控制器和其他分布在不同系统模块（被称为“卫星”控制器）的管理控制器

---
#### 组成
![bg right h:10cm](https://upload.wikimedia.org/wikipedia/commons/f/f2/IPMI-Block-Diagram.png)


* 同一设备内的卫星控制器通过称为智能平台管理总线/桥 (IPMB) 的系统接口连接到 BMC，这是 I²C 的一个增强实施。 BMC 通过智能平台管理控制器总线/桥(IPMC)连接到卫星控制器或另一个设备中的另一个 BMC。它可以通过远程管理控制协议 (RMCP) 进行管理。

---
##### BMC

![bg](https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/ASPEED_AST2400_BMC_Baseboard_management_controller.jpg/1920px-ASPEED_AST2400_BMC_Baseboard_management_controller.jpg)

---

## 我们来玩一玩 IPMI

---

## RTFM

![bg h:15cm](https://upload.wikimedia.org/wikipedia/commons/7/78/Demotivational_RTFM_Prudentia_Statue_on_the_Brussels_town_hall_%2853522136%29.jpg)
