# TextMiningAndAnalysis
Spec

## 01 Install VmWare instead of Virtual Box
* [VMware安装报VT-x未开启的解决办法](http://blog.163.com/jw_chen_cs/blog/static/202212148201361002518890/)
    * Because unknow host, I enter the BIOS and search for vitural technology and Intel-VT-x in every module(not in security).
   ```
   用虚拟机安装64位Ubuntu 12.04，然后出错，如下：
Thishost supports Intel VT-x, but Intel VT-x is disabled.

IntelVT-x might be disabled if it has been disabled in the BIOS/firmware settings orthe host has not been power-cycled since changing this setting.

(1)Verify that the BIOS/firmware settings enable Intel VT-x and disable ’trustedexecution.’

(2)Power-cycle the host if either of these BIOS/firmware settings have beenchanged.

(3)Power-cycle the host if you have not done so since installing VMwareWorkstation.

(4)Update the host’s BIOS/firmware to the latest version.

因为电脑是Intel 64bit CPU的，上面的意思说没有开启VT-x技术，要到BIOS里面修改设置。

好吧，在google上找到了以下解决方法。

本人台式组装机，重启开机按Del进入BIOS界面，按Enter进到CPU的设置，然后方向键滚动到“Intel  Virtualization Technology”，Enter键选择"Enable"， 按"Esc"回到BIOS主界面，选择Security，找到 Intel VT-d，改为"Enable"。 然后，保存设置并退出。
   ```
