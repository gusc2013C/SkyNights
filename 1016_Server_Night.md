# 企业级计算机硬件杂谈

我们称作“服务器”的电脑同样是由那么几大件组成，有同样的工作原理，可以使用同样的配件。但是数据中心里最多能有数十万台服务器，如果其中有太多出故障，轻则增加维护成本，重则造成重大经济损失。那么，具有“高可用性”设计的服务器会与我们的家用台式机有什么不同？为什么我们可以从二手市场放心地捡“洋垃圾”？主讲人将会从装机体验、内存、硬盘、电源、远程管理和RTFM这些方面做详细的介绍。

## "服务器" ("Server")

### "企业级"

免工具维护，冗余设计，热插拔

## 物理结构

### 分类

机架式(Rack)、塔式(Tower)和刀片式(Blade)

![Pic that contains all kinds of servers](https://www.racksolutions.com/news//app/uploads/Rack-server-and-blade-server-together.jpg)

#### 机架式(Rack)

![Dell R730 Front](https://i.dell.com/is/image/DellContent/content/dam/ss2/product-images/dell-enterprise-products/enterprise-systems/poweredge/poweredge-r730/pdp/server-poweredge-r730-pdp-ng-hero-static-v2.jpg?hei=402&qlt=90,0&op_usm=1.75,0.3,2,0&resMode=sharp&pscan=auto&fmt=pjpg)

![Dell R730 Back](https://i.dell.com/das/xa.ashx/global-site-design%20WEB/92612f85-41af-5daf-b5d7-030f7bf68796/1/OriginalJPG?id=Dell%2fProduct_Images%2fDell_Enterprise_Products%2fEnterprise_Systems%2fPowerEdge%2fPoweredge_R730%2fpdp%2fserver-poweredge-r730-pdp-love-02.jpg&qlt=100%2c0)

#### 塔式(Tower)

![Dell T640 Front](https://i.dell.com/is/image/DellContent//content/dam/ss2/product-images/dell-client-products/peripherals/dellemc_pet640_16x25_bezel_lf.psd?fmt=png-alpha&pscan=auto&scl=1&hei=402&wid=402&qlt=100,1&resMode=sharp2&size=402,402&chrss=full)

![Dell T640 Back](https://i.dell.com/is/image/DellContent//content/dam/images/products/servers/poweredge/t640/dellemc-pet640-16x25-b.psd?fmt=png-alpha&pscan=auto&scl=1&hei=402&wid=240&qlt=100,1&resMode=sharp2&size=240,402&chrss=full)

#### 刀片式(Blade)

![Blade Server](https://i.ebayimg.com/images/g/FkYAAOxyGxxSKdTM/s-l500.jpg)

![IBM](https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/IBM_HS20_blade_server.jpg/1920px-IBM_HS20_blade_server.jpg)

### 散热

风道设计 (Cover)

### 以 R730 为例

![R730 Configuration](https://cloud.tsinghua.edu.cn/seafhttp/files/d57715c2-0fe4-4837-939e-083859eab96a/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20003038.png)

![Front Panel](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20003249.png)

![Back Panel](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20003304.png)

## 组成单元

### 主板 (Motherboard)

### 中央处理器 (CPU)

#### Difference between server and PC CPU

频率较低-单核弱
核数高、缓存大-多核强
总线吞吐速率大

##### Intel

![Xeon](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20005952.png)

![Core](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20010157.png)

##### AMD

![EPYC](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20005912.png)

![Ryzen](https://cloud.tsinghua.edu.cn/thumbnail/6057def066574d83b9f6/1024/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-10-16%20010106.png)

### 内存 (Memory)

Thx rxgg!!!!

### 电源 (Power Supply Unit, PSU)

![PSU](https://snpi.dell.com/snp/images/products/large/en-us~750-ABBQ/750-ABBQ.jpg)

### 存储

#### SAS (Serial Attached SCSI)

接口向下兼容 SATA (Serial AT Attachment, Serial ATA)

![SATA and SAS](https://demartek.principledtechnologies.com/Images/SAS_SATA_Connectors.png)

##### Physica interface

![Mini-SAS Female](https://demartek.principledtechnologies.com/images/Mini_SAS_HD_compare-1.png)

![Mini-SAS Male](https://demartek.principledtechnologies.com/images/Mini_SAS_HD_compare-2.png)

SAS: 3 Gb/s in 2005, 6 Gb/s in 2009, 12 Gb/s in 2H 2013

SATA: 1.5 Gb/s in 2003, 3 Gb/s in 2005, 6 Gb/s in 2010 (traditional SATA is not expected to extend beyond 6 Gb/s)

##### Why SAS is better for servers and workstations

If you’re setting up a server for use by your office complex or small business, get servers and hard drives that use SAS technology. SAS is also a good component to have in your computer if you use your computer for processing-intensive work, like video editing, visual effects creation, or animation.
Here’s why SAS works well for servers and creative workstations.

###### Read/write speed

SAS is an all-around faster technology than SATA because it transfers data out of storage just as quickly as it transfers data into storage. Servers and workstations rely heavily on data transfer, so it’s good to have hardware that can send and receive information at a fast pace.
Storage capacity

SAS doesn’t have a storage capacity that’s as large as SATA, but it doesn’t need to. Servers utilize several different hard drives, so they’ll have the collective storage capacity of all the hard drives. And most creative professionals use multiple hard drives, anyway.

###### Price

SAS hardware is more complicated, and that makes it more expensive. On the bright side, SAS hardware is more durable than SATA. The MTBF (mean time before failure) of SATA is 1.2 to 1.6 million hours. That means that SATA tech is likely to run for well over a million hours before it needs to be replaced [7].

###### Smart tech

SAS is built with integrated technologies that make it especially useful for servers and workstations. Hard drives that are built with SAS connectors are cased in “SCSI enclosures.”

A SCSI enclosure is a piece of hardware that helps your hard drive manage the traffic that’s coming and going through the SAS highway. If there’s an error in the hardware, the SCSI enclosure programming can find it and report it.

#### RAID

The SCSI programming uses RAID to protect you from data loss. When you’re working with data that hasn’t been saved to storage, SCSI ensures that all data exists on multiple drives, so that if one drive fails, the data will still exist on another.

This process is called RAID (Redundant Array of Independent Disks). You can perform RAID on SATA technology, too, but it’s more efficient on SAS technology because SAS links more circuitry. Servers and workstations conduct so many transfers of temporary data that having RAID-capable technology is a necessity [8].

One final capability of SAS is that it allows for multipath input/output (I/O). Since SAS technology usually connects more than one piece of circuitry, it can reroute data through a secondary highway if the primary highway fails. This is an important feature to have in very large interconnected systems, like servers [9].

##### RAID controllers

![H730](https://snpi.dell.com/snp/images/products/large/en-us~490-BDUT/490-BDUT.jpg)

In hardware-based RAID, a physical controller is used to manage the RAID array. The controller can take the form of a PCI or PCI Express (PCIe) card, which is designed to support a specific drive format such as SATA or SCSI. (Some RAID controllers can also be integrated with the motherboard.) Hardware RAID controllers are also often referred to as RAID adapters.

A RAID controller may also be software-only, using the hardware resources of the host system, particularly the host’s CPU and DRAM. Software-based RAID generally provides similar functionality to hardware-based RAID, but its performance is typically less than that of the hardware versions.

#### SAS expanders

Components that facilitate communication between a large number of SAS devices, with these expanders having two or more external expansion ports. The expanders have at least one SAS management protocol destination port and can support SAS drives.

Expanders are not required to interconnect an initiator and SAS targets. At the same time, it enables a single initiator to communicate with more SAS / SATA targets. Its operation is similar to a network switch, allowing multiple systems to be connected using a single switched port.

![SAS Expander](https://t7m8e9c8.rocketcdn.me/wp-content/uploads/2020/02/raid-sas.jpg)

#### M.2, U.2 & NVMe

##### M.2

![M.2](https://ae01.alicdn.com/kf/H4ee7687701024be3899244d0a57ed1dfN/M-2-SSD-to-U-2-Adapter-2in1-M-2-NVMe-and-SATA-Bus-NGFF-SSD.jpg)

M.2 is the next generation PCIe connector that can be used for internally mounted devices such as boot drives in a variety of devices, from mobile to server. Its multiple socket definitions support WWAN, SSD and other applications. M.2 can support PCIe protocol or SATA protocol, but not both at the same time on the same device. M.2 supports a variety of board width and length options. M.2 is available in single-sided modules that can be soldered down, or single-sided and dual-sided modules used with a connector. M.2 PCIe is also available in a Ball Grid Array (BGA) form factor.

##### U.2

![U.2](https://demartek.principledtechnologies.com/Images/Demartek_SFF-8639.png)

U.2 (formerly SFF-8639) is the I/O backplane connector designed for high-density SSD storage devices and is backward compatible with existing storage interfaces. SFF-8639 supports PCIe/NVMe, SAS and SATA devices and enables hot plug and hot swap of devices while the system is running.

##### NVMe (Non-Volatile Memory Express)

The NVMe interface is the newest type of flash storage withthe highest performance. The driving architectural differentiator of NVMe is that it uses the PCIe interface bus to connect directly to the CPU and streamline the travel path. This design contrasts with SAS and SATA, which require data to first traverse to an HBA before reaching the CPU. By removing a layer from the stack, the travel path isoptimized and produces reduced latency and improved performance. Scalability is also significantly improved, becauseNVMe drives can go beyond the traditional four lanes by using lanes from the same “pool” of lanes connected to the CPU. Furthermore, NVMe performance will continually improve as each new generation of the PCIe standard becomes available.

### 智能平台管理接口 (Intelligent Platform Management Interface, IPMI)

原本是一种Intel架构的企业系统的周边设备所采用的一种工业标准。

1998年Intel、DELL、HP及NEC共同提出IPMI规格，可以透过网络远程控制温度、电压。

2001年IPMI从1.0版改版至1.5版，新增 PCI Management Bus等功能。

2004年Intel发表了IPMI 2.0的规格，能够向下兼容IPMI 1.0及1.5的规格。新增了Console Redirection，并可以通过Port、Modem以及Lan远程管理服务器，并加强了安全、VLAN 和刀片服务器的支持性。

#### 特性

IPMI独立于操作系统外自行运作，并容许管理者即使在缺少操作系统或系统管理软件、或受监控的系统关机但有接电源的情况下仍能远程管理系统。IPMI也能在操作系统启动后活动，与系统管理功能一并使用时还能提供加强功能，IPMI只定义架构和接口格式成为标准，详细实现可能会有所

#### 组成

![IPMI Block Diagram](https://upload.wikimedia.org/wikipedia/commons/f/f2/IPMI-Block-Diagram.png)

IPMI包含了一个以 基板管理控制器(BMC) 为主的控制器和其他分布在不同系统模块（被称为“卫星”控制器）的管理控制器，卫星控制器包含了相同的架构透过IPMB(Intelligent Platform Management Bus/Bridge) - 一个I²C (Inter-Integrated Circuit)加强实现的系统接口链接到基板管理控制器(BMC)，基板管理控制器(BMC) 也能与 远程管理控制协议(RMCP) - 一个在此规格内的特殊有线协议一同被管理。

##### BMC

![Fully integrated BMC as a single chip on a server motherboard](https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/ASPEED_AST2400_BMC_Baseboard_management_controller.jpg/1920px-ASPEED_AST2400_BMC_Baseboard_management_controller.jpg)

The baseboard management controller (BMC) provides the intelligence in the IPMI architecture. It is a specialized microcontroller embedded on the motherboard of a computer – generally a server. The BMC manages the interface between system-management software and platform hardware. BMC has its dedicated firmware and RAM.

Different types of sensors built into the computer system report to the BMC on parameters such as temperature, cooling fan speeds, power status, operating system (OS) status, etc. The BMC monitors the sensors and can send alerts to a system administrator via the network if any of the parameters do not stay within pre-set limits, indicating a potential failure of the system. The administrator can also remotely communicate with the BMC to take some corrective actions – such as resetting or power cycling the system to get a hung OS running again. These abilities reduce the total cost of ownership of a system.

## RTFM

Read The Fxxking Manual

![RTFM](https://upload.wikimedia.org/wikipedia/commons/7/78/Demotivational_RTFM_Prudentia_Statue_on_the_Brussels_town_hall_%2853522136%29.jpg)
