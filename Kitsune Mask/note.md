## R6566BB1C-kitsune

* *小心！您使用的Magisk版本未经Magisk官方开发人员批准。此版本可能有危险的更改，可能会损坏您的设备或暴露您的数据。不要向Magisk官方渠道寻求任何支持或报告任何问题。如果你正在使用这个版本而不知道它是非官方的，请切换到官方Magisk，网址为【github.com/topjohnwu/Magisk】(https://github.com/topjohnwu/Magisk)。使用这个你要自担风险！**

-修复使用SuList时注射“su”可能失败的问题(由@kitsunedfox报告)

### 与官方Magisk不同

- [Zygisk]通过ptrace注射受精卵(*)
-[常规]禁用Zygisk时，使用MagiskHide隐藏
-[常规]支持模块的预初始化挂载
-[常规]支持使用指定的空白字符设备(如KSU `overlayfs `等)删除文件
- [App]支持将Magisk安装到`/system `(用于仿真器)
-[守护程序]使用unix套接字通信

### 学分

- (*) Kitsune Mask正在使用来自[ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext)的部分代码，它是由[Dr-TSNG](https://github.com/Dr-TSNG/ZygiskNext)和[5 ec1 CFF](https://github.com/5ec1CFF)编写的开源项目，并在GPL-version 3.0下授权。[ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext)为KernelSU提供了Zygisk和Zygisk API支持的独立实现，并取代了Magisk的内置Zygisk。

### Magisk上游级别

- HEAD commit: ecb31ee