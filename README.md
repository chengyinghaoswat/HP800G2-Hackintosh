# HP800G2-Hackintosh

### 测试目前支持的版本为：Monterey 12.0.1正式版

#### 先说废话：

我又来了，这次带来的机器是惠普的800G2dm!

我总是热衷于这种mini机器，因为他真的很方便，体积小，性能也不算太差，相对于apple的mini电脑，性价比又真的很高！

![](/Users/eddy/Documents/GitHub/HP800G2-Hackintosh/image/front.jpg)

这个是机器的正面图！很前卫的是，竟然拥有一个Type-C的接口！

![back](/Users/eddy/Documents/GitHub/HP800G2-Hackintosh/image/back.jpg)

这个则是机器背部的接口，左侧的一个小盒子是外置的天线，接口很多，而且大部分都是USB3.0的接口，中间的口可以自己改装成HDMI的接口，不过毕竟是黑苹果，对HDMI的支持并没有那么好，而且一张转接卡要80元左右，对于我这种没有需求的人来说，就算啦！

#### 机器配置：

| 配件名称 | 型号                | 备注                             | 价格           |
| -------- | ------------------- | -------------------------------- | -------------- |
| CPU      | 酷睿i5-6600T        |                                  | 550            |
| 内存     | 昱炎DDR4 8G✖️2 26666 | 兼容性还不算差                   | 135✖️2          |
| 硬盘     | 雷克沙 480G nvme    | 咸鱼二手货                       |                |
| 网卡     | Bcm943224           | 有条件可以上其他博通卡，ngff接口 | 库存忘记价格了 |
| 准系统   | Hp800g2 dm          | 电源自己另买的                   | 310            |
| bios版本 | 02.53Rev.A          |                                  |                |

总体配置下来在1200RMB左右，当然还包括我上面没有提到的（电源，网卡转接卡，天线）

#### 安装设置：

如果你不想因为bios的版本不同，导致安装时出现了其他问题，请先将bios版本更新至与我相同，我已将bios安装包放在bios目录中，请自行更新！

1. 首先，你需要准备U盘和镜像，这里我就不提供了，独自完成写盘，替换EFI的操作。

2. 开机中按ESC键进入BIOS选项卡，选择BIOS Setup（F10）

   Advanced--->Boot Option

   ​						Fast Boot--->❌

   ​						Usb Storage Boot--->✔️

   Advanced--->Secure Boot Configuration

   ​						Configure Legacy Support and Secure Boot--->Legacy Support Disable and Secure Boot Disable

   Advanced--->System Options

   ​						Virtualization Technology(VTx)--->✔️

   ​						Virtualization Technology for DirectedI/O(VTd)--->❌

   Advanced--->Built-In Device Options

   ​						Video memory size--->64MB

   至此，bios设置设置完毕。

至于在后面如何操作，这里我就不一一赘述了，网上的教程很多，操作都是一样的！

本EFI已定制USB，并包括博通的蓝牙WIFI驱动，如果你的电脑没有博通网卡，请自行关闭驱动挂载！

ps：我在咸鱼上有售卖此类机器【黑果小x先生】
