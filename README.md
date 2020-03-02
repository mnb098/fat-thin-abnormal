# fat-thin-abnormal
study linux notes and others

问题：vmware安装fedora的时候总是出现错误提示

> end kernel panic： not syncing fatal exception in interrupt

解决方案1：

1. 确认VMware版本和虚拟机镜像版本兼容性！！！

 2. 修改配置文件：在你保存的这个虚拟机的目录下找到.vmx后缀的，用记事本打开将 firmware = "efi" 变成 firmware = "bios"

 3. 编辑虚拟机，显示器设置里去掉3D图形前面的勾选

解决方案2：

主要是开机进入到bios中，将选项“Onboard Lan”的选项“Disabled”掉，然后重启从光驱启动即可。

等安装完系统之后，再进入BIOS将“Onboard Lan”的选项给“enable”，否则网卡有可能会出问题！

FINALLY解决方案:安装了vm pro
