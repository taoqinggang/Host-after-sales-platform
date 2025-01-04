---
title: "雷神A8000路由器新特性"
date: 2024-12-17T00:00:00
tags: ["A8000"]
categories: ["雷神路由器"]
banner: "img/banners/banner-4.jpg"
baseurl: "http://118.126.104.235/"
---
### 新特性：

**1、优化热门游戏的下载速度和游戏延迟**

**2、支持vr、steamdeck设备加速**





------

### 附：硬件信息

#### cpu:

**CPU 型号**：ARM Cortex-A53 (ARMv8 架构)

**核心数**：2 核

**频率 (BogoMIPS)**：26.00

**架构**：ARMv8 64 位

**支持特性**：AES、SHA、浮点、SIMD 等。

```shell
root@OpenWrt:~# cat /proc/cpuinfo
processor       : 0
model name      : ARMv8 Processor rev 4 (v8l)
BogoMIPS        : 26.00
Features        : fp asimd evtstrm aes pmull sha1 sha2 crc32 cpuid
CPU implementer : 0x41
CPU architecture: 8
CPU variant     : 0x0
CPU part        : 0xd03
CPU revision    : 4

processor       : 1
model name      : ARMv8 Processor rev 4 (v8l)
BogoMIPS        : 26.00
Features        : fp asimd evtstrm aes pmull sha1 sha2 crc32 cpuid
CPU implementer : 0x41
CPU architecture: 8
CPU variant     : 0x0
CPU part        : 0xd03
CPU revision    : 4
```

#### 内存：

512 MB

```shell
root@OpenWrt:~# free -h
              total        used        free      shared  buff/cache   available
Mem:         492608      181000      271564       12328       40044      284900
Swap:             0           0           0
```

#### 存储：

**根文件系统 `/`**：挂载在 `/overlay`，大小 **68.7M**。

**只读根文件系统 `/rom`**：占用 **23.0M**。

```
root@OpenWrt:~# df -h
Filesystem                Size      Used Available Use% Mounted on
/dev/root                23.0M     23.0M         0 100% /rom
tmpfs                   240.5M     26.9M    213.6M  11% /tmp
/dev/ubi0_2              68.7M      7.0M     58.1M  11% /overlay
overlayfs:/overlay       68.7M      7.0M     58.1M  11% /
tmpfs                   512.0K         0    512.0K   0% /dev
```

