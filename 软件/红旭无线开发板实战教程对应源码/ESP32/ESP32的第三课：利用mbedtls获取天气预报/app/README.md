# 前言
> 这个是红旭无线开发板的第三课教程 **(ESP32的第三课：利用mbedtls获取天气预报)** 所对应的源码,主要是实现了通过按键切换不同城市然后再获取对应城市天气预报功能.

# 如何使用
用户只需要将 **app**这个文件夹复制至esp32 sdk的根目录下即可,无须做任何更改.但是,有一点还是需要注意一下;
- 如果在编译的过程中出现编译错误,只需要<cdoe>make app-clean</code>即可.出现这种情况的可能是因为编译的时候遗留了一些文件,而这些文件由于不同人把sdk存放的目录不同而不同
- 如果上面的动作编译没有问题,则再执行<code>make app-flash</code>即可烧录这一课的固件至你的开发板中去

# 功能
- 按键按照**北京**-->**上海**-->**广州**-->**深圳**这样的顺序获取对应城市当天以及未来两天的天气预报情况
- 呼吸灯对应上面城市颜色变化分别为R-->G-->B-->R
- 获取得到的天气预报信息均通过串口打印出来,串口的波特率为115200bps

# 最后
如何在使用上有什么问题,欢迎提Issues或者到[红旭对应的无线技术论坛](http://bbs.wireless-tech.cn/forum.php)提问.
