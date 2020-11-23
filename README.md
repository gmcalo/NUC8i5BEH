# NUC8I5BEH Hackintosh (OpenCore)
## NUC8（豆子峡谷）在线安装macOS

![Hackintosh](AboutThisMac.png)

### 关于在线更新11.0.1的方法
需要注意的是，这个EFI不支持在线更新到最新的11.0.1系统。
需要在线更新的方法，是安装好系统后，替换最新的支持11的EFI，再进行系统更新。
本人常识使用该项目的[EFI](https://github.com/csrutil/NUC8I5BEH)，顺利升级到最新的系统。


### 配置
+ OS: macOS Catalina 10.15.7 19H2 x86_64 / Macmini8,1
+ OpenCore: 0.6.2
+ CPU: Intel® Core™ i5-8259U Processor (6M Cache, up to 3.80 GHz)
+ SSD: 500GB HP EX900系列
+ RAM: 16GB x 1 ￼光威（Gloway）16GB DDR4 2666频率 战将系列
+ BIOS: 0085
+ Monitor: AOC 27英寸 Q2790PQ

#### SP：采购的机器是SD卡硬改的全新NUC8I5BEH厚版

### BIOS设置
+ __Disable__
	- Legacy Boot
	- Fast Boot
	- Network Boot
	- Secure Boot
	- Inter VT for directed I/VO(VT-d)
+ __Enable__
	- Boot USB Devices First
	- Boot Network Devices Last
+ __Wake on LAN from S4/S5__
	- Stay Off


### 制作U盘启动盘
+ 使用diskginues把U盘格式化为FAT32文件系统（不格式化为FAT32的话我进不去uefi引导）
+ 将 **EFI** 和 **NUC8_MacOnlineInstaller** 两个文件夹放入U盘根目录，执行**NUC8_MacOnlineInstaller**中的run脚本，完成后使用U盘开机即可安装
+ 其他安装流程跟网上一模一样，[详见](https://www.jianshu.com/p/78510cfa4a64)


### 安装心情记录
+ 安装后完美使用，是最新的10.15.7版本，感觉终于用上全家桶了
+ 能够完美使用Wi-Fi，蓝牙，airdrop，随航。还能无缝连我的AirPods2
+ 后悔选择2K屏幕了，感觉字体小，改分辨率又模糊，不想修改HIDPI，还是换个4k屏幕吧
+ 这个在线安装黑苹果的方法绝对是最省心的。os镜像需要在线下载，学校的网速又慢，于是选择睡觉前安装，打开扔着，早上睡醒就进入新系统设置界面了
+ 开放这个脚本的好像要收费，但我是从Github fork下来的，算是白嫖吧～
