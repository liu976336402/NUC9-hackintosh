### 硬件信息
- nuc9i9qnx(理论上nuc9全系通用 包括幽灵峡谷 石英峡谷)
- 无线网卡: 板载intelax200网卡
- 内存: 英睿达 3200MHz 16GBx2 DDR4
- 显卡: 6600xt 免驱
- 硬盘: PREDATOR Gm7000 1000GB
- 声卡: 板载ALC256

![About](/pic/about.png)

### opencore
- opencore版本 0.8.3 
- 仿冒型号 iMac19,1

### 目前状态

基本完善，满足日常使用

#### 已经完善

* [x] 板载的intel无线网卡，速度还不错
![Speedtest](/pic/speedtest.jpg)
* [x] 核心显卡已经驱动但是用的目前的efi中仅作为计算使用，不能驱动输出
* [x] 独立显卡Readon 6600xt
* [x] USB接口已经定制，所有usb接口均可以使用
* [x] 声卡驱动正常
* [x] 休眠/唤醒正常
* [x] 蓝牙正常
* [x] 双网口驱动正常
![Bluetooth](/pic/bluetooth.png)

#### 未完善
* [ ] 读卡器没有sd卡测试，但是这个读卡器走的是USB3.2的hub，理论上应该可以使用
* [ ] 雷电三载系统信息中能看到，但是手中没有硬件可以测试

### 其他
- 启动阶段会有一小段时间黑屏，但是不影响启动
- 关于更换白苹果网卡以后在Montery中蓝牙无法使用的问题 请移步国光大佬的博客 [国光的黑苹果安装教程](https://apple.sqlsec.com/) 
    - 自行定制usb [定制usb](https://apple.sqlsec.com/6-%E5%AE%9E%E7%94%A8%E5%A7%BF%E5%8A%BF/6-1/)
    - 更换kext文件 [macos12蓝牙](https://apple.sqlsec.com/6-%E5%AE%9E%E7%94%A8%E5%A7%BF%E5%8A%BF/6-7/) 


### 更新记录
- 2022/7/29 升级至opencore0.8.2 系统无痛升级到Monterey 12.5
![Monterey12.5](/pic/12.5.png)
- 2022/8/26 升级至opencore0.8.3 系统无痛升级到Monterey 12.5.1
![Monterey12.5.1](/pic/12.5.1.png)
- 2022/10/25 升级至opencore0.8.5 系统无痛升级到Monterey 12.6
本次升级使用ocat工具升级 建议使用u盘放入新的efi并更换自己的三码后 使用u盘引导开机测试 成功后在替换磁盘efi分区中的efi文件
![Monterey12.6](/pic/Monterey12.6.jpg)