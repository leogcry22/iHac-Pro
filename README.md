# 介绍

长期不定期维护，我的工作用黑苹果OpenCore配置指南，硬件升级空间灵活

P.S. 本人非大神，闲暇之余慢慢摸索学习OC中，此EFI仅供满足本人日常使用，并非所有功能均完善，OC配置文件也非100%正确，套用之前请确保已阅读下列内容并正确完成相关设置，若有问题可提交至[Issues](https://github.com/leogcry22/iHac-Pro/issues)中

> 另外也欢迎同配置的朋友与我共同维护此项目

## 目录

- [预览](#预览)
- [不兼容硬件](#不兼容硬件)
- [配置](#配置)
- [组装建议](#组装建议)
- [SMBIOS](SMBIOS)
- [开始之前](#开始之前)
- [BIOS设置](#BIOS设置)
- [注意事项](#注意事项)
- [已知正常工作](#已知正常工作)
- [已知/未知不工作](#已知/未知不工作)
- [参考](#参考)

## 预览

![showcase](Images/showcase.jpg)

## 配置

| 硬件 | 型号 | 说明 |
| :---: | --- | --- |
| 处理器 | 英特尔 酷睿 i5-9600KF | 稳定超频至5.0GHz |
| 主板 | 技嘉 Z390M Gaming |
| 内存 | 科赋 DDR4 2666MHz 16GB 普条 * 2| CJR颗粒，稳定超频至3600MHz |
| 显卡 | 蓝宝石 RX 5500 XT 白金版 OC |
| 固态硬盘1 | 西部数据 SN500 500GB| macOS |
| 固态硬盘2 | 西部数据 SN500 500GB| Windows 10 |
| 机械硬盘 | 东芝 P300 3TB |
| 散热器 | 九州风神 大霜塔 RGB |
| 机箱风扇 | 九州风神 魔环 RGB |
| 机箱 | 乔思伯 C3-Plus |
| 电源 | 海盗船 RM650X |
| 网卡&蓝牙 | 无 | 目前暂无需求，可自行加装白果网卡或兼容型号 |

## 组装建议
- 处理器：理论上只要是9代无核显版本的任何型号CPU都支持，合理配置散热即可
- 显卡：目前已知RDNA架构5500XT与5700XT都支持，5600XT目前待测
- 主板：不保证能套用至其它厂商的其它型号，也许技嘉自家的系列可以
- 固态硬盘：除了三星家的OEM盘PM981/PM981a有兼容问题之外，其余均可
- 仓库盘：为以防万一，建议加装一块仓库盘用于Time Machine备份
- 无线网卡：有需要可以加装白果的免驱卡或者兼容的网卡进行配置
- 其它：选择自己中意的就行，不会有什么太大影响

## SMBIOS

  `iMacPro1,1`

## 开始之前

BIOS版本：[**`F9g`**](https://www.gigabyte.com/Motherboard/Z390-M-GAMING-rev-10/support#support-dl-bios)

**请务必确保CFG Lock已解锁！！！**

**请务必确保CFG Lock已解锁！！！**

**请务必确保CFG Lock已解锁！！！**

> 解锁方式有多种，个人这里采用的为直接修改BIOS文件并刷入主板的方式，你也可以采用其它任何方式

## BIOS设置

## 注意事项

**安装前请务必使用工具生成三码并填入[`EFI/OC/config.plist`](https://github.com/leogcry22/iHac-Pro/blob/master/EFI/OC/config.plist)中**

## 已知正常工作

* [x] CPU变频
* [x] GPU硬件加速
* [x] 音频输入与输出
* [x] 睡眠与唤醒
* [x] 有线网络
* [x] USB

## 已知/未知不工作

* [ ] 原生NVRAM（WIP）
* [ ] 系统定位（需要无线网卡）
* [ ] 更多未知问题？请提交至[Issues](https://github.com/leogcry22/iHac-Pro/issues)中

## 参考

- [OpenCore Vanilla Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)

- [使用OpenCore引导黑苹果](https://blog.xjn819.com/?p=543)

- [精解OpenCore](https://blog.daliansky.net/OpenCore-BootLoader.html)

- [技嘉神板回归！BIOS解锁CFG Lock！！！](https://bbs.pcbeta.org/viewthread-1835794-1-1.html)
