**English** | [中文](/README.md)
## HP Pavilion--16-a0001tx-Hackintosh
[![Release](https://img.shields.io/github/v/release/zzzyy678/-Pavilion--16-a0001tx-Hackintosh?label=Release)](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/releases)

<img src="img/Machine.png" width="400" height="400"/> 

- macOS10.15 Catalina：`OpenCore v0.6.8`  
  - [Download EFI](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/releases/download/v0.6.8-oc/OCv0.6.8Catalina.zip)
- macOS12 Monterey&macOS13 Ventura：`OpenCore v0.8.8`  
  - [Download EFI](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/releases/download/v0.8.0-oc/OC.v0.8.8.zip)
### Preparation before installing macOS：CFG-Unlock & Set DVMT to 64MB
Boot on[CFG-Lock.zip](https://github.com/zzzyy678/-Pavilion--16-a0001tx-Hackintosh/raw/main/CFG-Unlock.zip)BOOTX64.EFI，enter the following two commands：
```shell
setup_var 0x3e 0x01
setup_var 0xf5 0x2
```
### Open HIDPI
```shell
bash -c "$(curl -fsSL https://raw.githubusercontent.com/xzhih/one-key-hidpi/master/hidpi.sh)"
```
Or download [one-key-hidpi](https://github.com/xzhih/one-key-hidpi/archive/refs/heads/master.zip) running`hidpi.command`

-----
### Configuration

| Specifications      | Detail                                 | PS |
| -------- | ---------------------------------------- | --- |
| 电脑型号 | HP Pavilion-16-a0001tx | 完成度96% |
| 处理器 | Intel Core i7-10750H | 已驱动变频 |
| 内存 | 三星 DDR4 16GB 2933MHz  | 识别正常 |
| 硬盘 | WDC Nvme SN720 512GB | 识别成PCIE硬盘，外接SATA正常 |
| 核显 | Intel UHD Graphics 630 | 核显硬解正常，已开启平滑亮度调节 |
| 独显 | NVIDIA Geforce RTX2060 MAX-Q | 无解，已屏蔽 |
| 声卡 | 瑞昱 ALC245 | 智音麦克风无解；注入layout-id：11 |
| 无线网卡 | Intel AX201 | 建议更换博通 BCM94352z |
| 有线网卡 | 瑞昱 RTL8111 | 内建驱动正常 |
| 触控板 | ELAN072E | 已定制驱动，多指正常 |
| 传感器 | 温度传感器 | 已注入双风扇显示转速|


