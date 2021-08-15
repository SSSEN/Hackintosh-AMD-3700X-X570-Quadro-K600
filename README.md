# Hackintosh-AMD-3700X-X570-Quadro-K600

WIN/MAC 双系统 双显卡 双SSD
WIN下使用6700XT
MAC下使用K600
无需插拔显卡，根据需要在对应显卡上连接显示器

| Type          | Name   |
| --------      | -----  |
|macOS          |   11.5.2 (20G95) |
|SMBIOS         |   iMac Pro|
| CPU           |   AMD 3700X |
| GPU           |   NVIDIA Quadro K600 / AMD RX 6700XT  |
| MB            |   TUF GAMING X570-PLUS |
| NVME          |   WD SN750 / WD SN550  |
|WIFI           |   Broadcom 免驱网卡 |


其他CPU需要修改核心计数补丁来引导系统。找到三个algrey - Force cpuid_cores_per_package补丁并只更改Replace值。

将 B8000000 0000/BA000000 0000/BA000000 0090*  更改为B8 <核心数> 0000 0000/BA <核心数> 0000 0000/BA <核心数> 0000 0090*
用与您的物理核心计数匹配的十六进制值替换<核心数>。
 
| 核心          | 替换数值   |
| --------      | -----  |
|4 Core	|04|
|6 Core	|06|
|8 Core	|08|
|12 Core	|0C|
|16 Core	|10|
|24 Core	|18|
|32 Core	|20|

# 正常工作

 - [x] Wi-Fi
 - [x] 蓝牙
 - [x] 有线网络
 - [x] 音频
 - [x] Airdrop
 - [x] 显示器 LG 27UL650 4k
 - [x] USB 3.1

# 未正常工作

 - [ ] 睡眠
 - [ ] HDR （K600不支持 HDR）

 
