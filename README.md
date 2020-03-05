# 介绍

长期不定期维护，我的黑苹果OpenCore配置，灵活预留了升级空间

P.S. 本人非大神，闲暇之余慢慢摸索学习OC中，此EFI仅供满足本人日常使用，并非所有功能均完善，OC配置文件也非100%正确配置，套用之前请确保已阅读下列内容并正确完成相关设置，若有问题可提交至[Issues](https://github.com/leogcry22/iHac-Pro/issues)中

> 另外也欢迎同配置的朋友与我共同维护此项目

### 目录

- [预览](#预览)
- [不兼容硬件](#不兼容硬件)
- [配置](#配置)
- [组装建议](#组装建议)
- [开始之前](#开始之前)
- [BIOS设置](#BIOS设置)
- [注意事项](#注意事项)
- [已知正常工作](#已知正常工作)
- [已知/未知不工作](#已知/未知不工作)
- [参考](#参考)

### 预览

### 配置

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
| 无线网卡 | 无 | 目前暂无需求，可自行加装白果网卡或兼容型号 |

### 组装建议

CPU：

### 开始之前

BIOS版本：[`F9g`](https://www.gigabyte.com/Motherboard/Z390-M-GAMING-rev-10/support#support-dl-bios)

**请务必确保CFG Lock已解锁！！！**

**请务必确保CFG Lock已解锁！！！**

**请务必确保CFG Lock已解锁！！！**

> 解锁方式有多种，个人这里采用的为直接修改BIOS文件并刷入主板的方式，你也可以采用其它任何方式

### BIOS设置

### 注意事项

### 已知正常工作

* [x] CPU变频
* [x] GPU硬解
* [x] 音频输入与输出
* [x] 睡眠与唤醒
* [x] 网络
* [x] USB

### 已知/未知不工作

* [ ] 原生NVRAM（WIP）
* [ ] 系统定位（需要无线网卡）
* [ ] 更多未知问题？请提交至[Issues](https://github.com/leogcry22/iHac-Pro/issues)中

### 参考

- [OpenCore Vanilla Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)

- [使用OpenCore引导黑苹果](https://blog.xjn819.com/?p=543)

- [精解OpenCore](https://blog.daliansky.net/OpenCore-BootLoader.html)

- [技嘉神板回归！BIOS解锁CFG Lock！！！](https://bbs.pcbeta.org/viewthread-1835794-1-1.html)
