大家好我来自中国的菜鸟极客 DJY（打酱油...）今天我给大家带来一份情人节礼物。就是oneplus6 or 6t 的nethunter内核。大家好我来自中国的菜鸟极客 DJY（打酱油...）今天我给大家带来一份情人节礼物。就是oneplus6 or 6t 的nethunter内核。
修复全功能支持。支持网卡 RTX系列 ，联发科mtu7601u系列，修复了RTL-SDR功能支持，修复了hackrf one 支持 ，修复了HID 攻击 支持（感谢@simonpunk提供对HID的大力帮助，非常感谢），修复了simonpunk代码 nethunter app 对oneplus 6和6T支持（项目代码：https://github.com/simonpunk/nethunter-app）在项目新的代码中@simonpunk添加了
对自动生成对各种架构的kali 平台支持 arm arm64 amd64 armhf （项目代码：https://github.com/pelya/android-keyboard-gadget） ，添加了CP210x，FTDI，CH341 模块（现在你可以使用OTG+C118+osmocombb项目代码来进行GSM嗅探）。解锁了AM/FM 模块 现在你可以不使用SDR就可以接收AM/FM信号（大部分手机都内置AM/FM芯片，由于环境原因我没有进行测试。如果你需要测试可以用NextRadio APP 进行测试）
对@rithvikvibhu WIFI支持模块 进行略微修改。添加了 蓝牙 键盘攻击模块的支持。
构建内核代码:https://gitlab.com/HolyAngel/op6 感谢@HolyAngel 的优秀内核项目

nethunter app 构建代码：https://github.com/simonpunk/nethunter-app 感谢@simonpunk 对HID 攻击模块 提供大力帮助

magisk WIFI支持模块 来自@rithvikvibhu 感谢rithvikvibhu做出的贡献

内核使用以上项目的最新代码来构建
内核下载链接：https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel
HID攻击模块测试视频：https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/raw/master/4.x%E4%BB%A5%E4%B8%8A%E5%86%85%E6%A0%B8HID%E6%B5%8B%E8%AF%95%E8%A7%86%E9%A2%91.webm

以下是测试截图：
[IMG]https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/blob/master/Screenshot_20190214-234924.jpg[/IMG]
[IMG]https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/blob/master/Screenshot_20190214-234952.jpg[/IMG]
[IMG]https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/blob/master/Screenshot_20190214-235038.jpg[/IMG]
[IMG]https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/blob/master/Screenshot_20190214-235114.jpg[/IMG]
[IMG]https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/blob/master/Screenshot_20190214-235217.jpg[/IMG]
[IMG]https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/blob/master/Screenshot_20190214-235240.jpg[/IMG]

使用说明：
关于usbarmy 的模块的使用说明可以参考这个链接，上面有详细的使用说明

下载官方最新https://twrp.me/Devices/ oneplus6 or 6t twrp
使用adb push kernel.zip  /sdcard/   刷入（已经内置了magisk） 或者使用 adb sideload 推送刷入

然后重启两次，打开magisk>模块>添加我修改后的WIFI支持包（已经内置nethunter等app）
