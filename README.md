## ASUS B360M-PLUS GAMING S OpenCore EFI

OpenCore版本： 0.6.7发行版
MacOS版本： Big Sur 11.2.3 

## 我的配置

| Type  | Model |
| ------ | ------ |
| CPU | Intel Core ~~i3 8100~~  i9 9900k |
| 主板 | ASUS TUF B360M-PLUS GAMING S |
| 内存 | 芝奇幻光戟 8G 3000MHz |
| 固态硬盘 | HP SSD EX900 M.2 250GB |
| 显卡 | ~~XFX Radeon RX570 4GB~~  Intel UHD Graphics 630 |


AMD涨价了，就把570卖了。
现在核显输出，B360主板HDMI/DVI无法输出问题不会搞，借用了[NEEPUCS](https://github.com/NEEPUCS)的[Ausu-ROG-Strix-B360i-HACKINTOSH-OPENCORE-EFI](https://github.com/NEEPUCS/Ausu-ROG-Strix-B360i-HACKINTOSH-OPENCORE-EFI)中的设置。
现在HDMI可以点亮屏幕，手头没有DVI显示器没有测试。但是不能设置休眠或者显示器休眠，屏幕黑了就无法亮了，只有重启了。


## Bios Setting
 
*English*    

- Boot>Boot Configuration >Fast Boot ： ***Disable***
- Boot>CSM(Compatibility Support Module)>launch CSM：***Disable***
- Boot>Secure Boot>OS type：***Other OS***
- Advanced>CPU Configuration >Software Guard Extensions(SGX)：***Disable***
- Advanced>CPU Configuration>CPU-Power Management Control >CFG lock：***Disable***
- Advanced >System Agent(SA) Configuration >VT-d：***Disable***
- Advanced >System Agent(SA) Configuration>Above 4G Decoding：***Enable***
- Advanced>PCH Configuration >System time and Alarm Source：***Legacy RTC***
- Advanced>USB Configuration >XHCI hand-off：***Enable***



*简体中文*    

* 启动>启动设置>快速启动：***关闭***
* 启动>CSM（兼容性支持模块>开启CSM：***关闭***
* 启动>安全启动菜单>操作系统类型 ：***其他操作系统***
* 高级>cpu设置>Software Guard Extensions(SGX)：***关闭***
* 高级>cpu设置>CPU-Power Management Control >CFG lock：***关闭***
* 高级>北桥>VT-d：***关闭***
* 高级>北桥>大于4G地址空间解码：***开启***
* 高级>PCH设置>System time and Alarm Source：***Legacy RTC***
* 高级>USB Configuration>XHCI hand-off：***开启***
