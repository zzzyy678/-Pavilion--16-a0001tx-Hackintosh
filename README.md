**中文** | [English](/README_EN.md)
## 惠普光影精灵6 Max 黑苹果
[![Release](https://img.shields.io/github/v/release/zzzyy678/-Pavilion--16-a0001tx-Hackintosh?label=Release)](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/releases)

<img src="img/Machine.png" width="500" height="500"/> 

- macOS10.15 Catalina：`OpenCore v0.6.8`  
  - [下载EFI](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/releases/download/v0.6.8-oc/OCv0.6.8Catalina.zip)
- macOS12 Monterey & macOS13 Ventura：`OpenCore v0.8.8`  
  - [下载EFI](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/releases/download/v0.8.0-oc/OC.v0.8.8.zip)
### 安装前准备：解锁CFG-Lock、设置DVMT为64MB 
启动[CFG-Lock.zip](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/raw/main/CFG-Unlock.zip)里的EFI，输入以下两条命令：
```shell
setup_var 0x3e 0x01
setup_var 0xf5 0x2
```
### 建议开启HIDPI
在终端输入以下命令回车
```shell
bash -c "$(curl -fsSL https://raw.githubusercontent.com/xzhih/one-key-hidpi/master/hidpi.sh)"
```
或者下载[one-key-hidpi](https://github.com/xzhih/one-key-hidpi/archive/refs/heads/master.zip) 双击`hidpi.command`运行

-----
### 电脑配置

| 硬件      | 详细信息                                  | 备注 |
| -------- | ---------------------------------------- | --- |
| 电脑型号 | HP Pavilion-16-a0001tx | 完成度96% |
| 处理器 | Intel Core i7-10750H | 已驱动变频 |
| 内存 | 三星 DDR4 16GB 2933MHz  | 识别正常 |
| 硬盘 | WDC Nvme SN720 512GB | 已开启TRIM，加装SATA识别正常 |
| 核显 | Intel UHD Graphics 630 | 核显硬解正常，已开启平滑亮度调节 |
| 独显 | NVIDIA Geforce RTX2060 MAX-Q | 无解，已屏蔽 |
| 声卡 | 瑞昱 ALC245 | 智音麦克风无解；注入layout-id：11|
| 无线网卡 | Intel AX201 | 建议更换奋威 DW1560 |
| 有线网卡 | 瑞昱 RTL8111 | 内建驱动正常 |
| 触控板 | ELAN072E | 已定制驱动，多指正常 |
| 传感器 | 温度传感器 | 已注入双风扇显示转速|

