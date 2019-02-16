大家好我来自中国的菜鸟极客 DJY（打酱油...）今天我给大家带来一份情人节礼物。就是oneplus6 or 6t 的nethunter内核。
修复全功能支持。支持网卡 RTX系列 ，联发科mtu7601u系列，修复了RTL-SDR功能支持，修复了hackrf one 支持 ，修复了HID 攻击 支持（感谢@simonpunk提供对HID的大力帮助，非常感谢），修复了simonpunk代码 nethunter app 对oneplus 6和6T支持（项目代码：https://github.com/simonpunk/nethunter-app）在项目新的代码中@simonpunk添加了
对自动生成对各种架构的kali 平台支持 arm arm64 amd64 armhf （项目代码：https://github.com/pelya/android-keyboard-gadget） ，添加了CP210x，FTDI，CH341 模块（现在你可以使用OTG+C118+osmocombb项目代码来进行GSM嗅探）。解锁了AM/FM 模块 现在你可以不使用SDR就可以接收AM/FM信号（大部分手机都内置AM/FM芯片，由于环境原因我没有进行测试。如果你需要测试可以用NextRadio APP 进行测试）
对@rithvikvibhu WIFI支持模块 进行略微修改。添加了 蓝牙 键盘攻击模块的支持。
构建内核代码:https://gitlab.com/HolyAngel/op6 感谢@HolyAngel 的优秀内核项目
测试机oneplus6T：测试系统 OOS bate 4

nethunter app 构建代码：https://github.com/simonpunk/nethunter-app 感谢@simonpunk 对HID 攻击模块 提供大力帮助

magisk WIFI支持模块 来自@rithvikvibhu 感谢rithvikvibhu做出的贡献

内核使用以上项目的最新代码来构建
内核下载链接：https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel
HID攻击模块测试视频：https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/raw/master/4.x%E4%BB%A5%E4%B8%8A%E5%86%85%E6%A0%B8HID%E6%B5%8B%E8%AF%95%E8%A7%86%E9%A2%91.webm

以下是测试截图：
![7](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-234924.jpg)
![8](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-234952.jpg)
![9](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235038.jpg)
![10](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235114.jpg)
![11](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235217.jpg)
![1](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235240.jpg)
使用说明：
关于usbarmy 的模块的使用说明可以参考这个链接，上面有详细的使用说明：https://forum.xda-developers.com/oneplus-5/development/burgerhunter-t3638810

下载官方最新https://twrp.me/Devices/ oneplus6 or 6t twrp
使用adb push kernel.zip  /sdcard/   刷入（已经内置了magisk） 或者使用 adb sideload 推送刷入

然后重启两次，打开magisk>模块>添加我修改后的WIFI支持包（已经内置nethunter等app）

现在你就可以完美使用nethunter内核。
问题反馈联系方式：Telegram:https://t.me/nethunter666 
github https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel
kali linux QQ群：891225998（欢迎各路大佬萌新进群吹水）
我会不定期更新，请给我一个start
关于编译这个内核我进行了上百次测试，如需转载还请注明出处。
如果你支持我的项目请给我一个star


English：
Hello everyone, I am a rookie geek from China DJY (soy sauce...) Today I will bring you a Valentine's Day gift. It is the nethunter kernel of oneplus6 or 6t.
Fix full feature support. Support network card RTX series, MediaTek mtu7601u series, fixed RTL-SDR function support, fixed hackrf one support, fixed HID attack support (thanks to @simonpunk for providing great help to HID, thank you very much), fixed simonpunk code nethunter app Oneplus 6 and 6T support (project code: https://github.com/simonpunk/nethunter-app) added simonpunk in the new code of the project
Added automatic support for the kali platform for various architectures arm arm64 amd64 armhf (project code: https://github.com/pelya/android-keyboard-gadget), added CP210x, FTDI, CH341 Module (now you can use the OTG+C118+osmocombb project code for GSM sniffing). Unlocking the AM/FM module Now you can receive AM/FM signals without using SDR (most phones have built-in AM/FM chips, I haven't tested them for environmental reasons. If you need testing you can test with NextRadio APP)
Make minor modifications to the @rithvikvibhu WIFI Support Module. Added support for the Bluetooth Keyboard Attack Module.
Nethunter app build code: https://github.com/simonpunk/nethunter-app Thanks to @simonpunk for providing great help to the HID attack module
Test machine oneplus6T: test system OOS bate 4
Build the kernel code: https://gitlab.com/HolyAngel/op6 Thanks to @HolyAngel for the excellent kernel project

Magisk WIFI support module from @rithvikvibhu Thanks to the contribution of rithvikvibhu

The kernel is built using the latest code from the above project
Kernel download link: https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel
HID attack module test video: https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/raw/master/4.x%E4%BB%A5%E4%B8%8A%E5%86%85%E6%A0%B8HID%E6%B5%8B%E8%AF%95%E8%A7%86%E9%A2%91.webm

The following is a test screenshot:
![7](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-234924.jpg)
![8](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-234952.jpg)
![9](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235038.jpg)
![10](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235114.jpg)
![11](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235217.jpg)
![1](https://raw.githubusercontent.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel/master/Screenshot_20190214-235240.jpg)
Instructions for use:
Instructions for using the usbarmy module can refer to this link for detailed instructions: https://forum.xda-developers.com/oneplus-5/development/burgerhunter-t3638810

Download the official latest https://twrp.me/Devices/ oneplus6 or 6t twrp
Use adb push kernel.zip /sdcard/ to brush in (magisk already built in) or use adb sideload to push in

Then restart twice, open magisk> module> add my modified WIFI support package (already built nethunter app)

Now you can use the nethunter kernel perfectly.
Feedback Contact: Telegram: https://t.me/nethunter666
Github https://github.com/johanlike/Oneplus6-or-6T-Nethunter-Kernel
Kali linux QQ group: 891225998 (welcome all the way big 佬 萌 new into the group blowing water)
I will update it from time to time, please give me a start
I have conducted hundreds of tests on compiling this kernel. Please indicate the source if you need to reprint.
If you support my project, please give me a star.
