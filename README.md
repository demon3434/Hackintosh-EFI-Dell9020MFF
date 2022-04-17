# Hackintosh-EFI-Dell9020MFF
## 戴尔9020MFF，黑苹果EFI

### 软件版本
| 软件 | 版本 |
| --- | :--: |
| 系统 | macOS Monterey 12.3.1 (21E258) |
| 引导 | OpenCore v0.7.9 |

### 自选硬件
|   硬件    |   型号  |
| -------- | :----: |
| 主机 | Dell OptiPlex 9020 MFF |
| CPU | Intel Core i5 4690T |
| 内存 | 英睿达 DDR3 1600 4G*2 |
| 硬盘 | 创见MTS420S NGFF接口（Sata协议） 120GB |
| 显卡 | Intel UHD Graphics 4600 |
| 显示器 | DIY便携屏，4K 60Hz |
| 无线网卡 | 白苹果拆机 BCM943224 |

### 完成度
+ 核显正常驱动，2048MB显存
+ 声卡可以驱动
+ Wi-Fi、蓝牙正常驱动，由于是白苹果拆机网卡，隔空投送完美（Big Sur下免驱动，Monterey下需要结合博通网卡驱动）
+ HDMI、DP接口均能亮屏，VGA接口未测试
+ 睡眠可唤醒
+ USB定制，所有USB接口正常
+ Sata硬盘装Win10，OC可引导Win10
+ 引导界面图形化，开机有“duang”声音

### 缺陷
+ 刚开机，两轮启动，苹果logo之后，偶尔会有屏幕熄灭的情况，但晃一晃鼠标，屏幕就亮了，可以能正常输密码登录系统

### 备注
1. PlatformInform 模拟机型，选择 iMac16,2
2. 由于本人使用4K显示器，故设置了UIScale=02；如果用1080P显示器，苹果logo会显得巨大，请自行到nvram的“4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14”中，修改UIScale为01
3. 如需使用此EFI，请***务必重新三码摇号***（适合OpenCore v0.7.9的OCC编辑器已放入本仓库，[图文教程](https://blog.csdn.net/xuanxue11/article/details/107873835)）

### 效果图
![关于本机.png](https://github.com/demon3434/Hackintosh-EFI-Dell9020MFF/blob/main/OpenCore%20v0.7.9%20%26%20macOS%20Monterey%2012.3.1%20(21E258)/1.%E5%85%B3%E4%BA%8E%E6%9C%AC%E6%9C%BA.png "关于本机")
![Hackintool系统信息.png](https://github.com/demon3434/Hackintosh-EFI-Dell9020MFF/blob/main/OpenCore%20v0.7.9%20%26%20macOS%20Monterey%2012.3.1%20(21E258)/2.Hackintool%E7%B3%BB%E7%BB%9F%E4%BF%A1%E6%81%AF.png "Hackintool系统信息")
