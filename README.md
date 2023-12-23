# wmt_mt7688_study
My MT7688 study

## Omega2+    
* 开源软件和硬件资料：https://github.com/OnionIoT    
Omega2系列核心板使用说明：https://docs.onion.io/omega2-docs/index.html  
实战项目：https://docs.onion.io/omega2-project-book-vol1/index.html  
论坛地址：https://community.onion.io/  
国内的论坛：https://cn.onion.io/  
官方网站：https://onion.io/  
开源软件和硬件资料：https://github.com/OnionIoT  
* 我看到omega2的文档，好像现在支持直接在设备上gcc了，嗯，这有点帅，  
omega2+的内存是128MB，omega2则是64MB，能跑得动gcc也是神奇  
（很容易内存不足挂掉），我想arm9是不是也能试试。。。  

## Omega2+ SSH  
* Wifi connection    
Wifi: omega-xxxx  
Password: 12345678  
See https://docs.onion.io/omega2-docs/first-time-setup.html  
**After this, use browser or use putty**    

* Use browser  
http://192.168.3.1  
User: root  
Pass: onioneer  
See https://docs.onion.io/omega2-docs/first-time-setup.html  

* Use SSH (use putty)     
IP: 192.168.3.1  
User: root  
Pass: onioneer  
See https://docs.onion.io/omega2-docs/first-time-setup-command-line.html  
$ wifisetup  

## Onion OpenWrt  
* https://github.com/OnionIoT/source  
* https://github.com/jslink/openwrt-trunk-dl  
* http://openwrt.bjbook.net/download/index.html  
* https://git.openwrt.org  
* make -j1 V=s  
* http://gw.stasoft.net/dl/  
* https://github.com/mhei/libugpio  
* https://github.com/OnionIoT/c-cross-compile-example/  
* https://github.com/OnionIoT/OpenWRT-Packages/tree/master/gpio-test  
* https://openwrt.org/docs/guide-developer/build-system/install-buildsystem  
* https://github.com/akmaker/openwrt-cn/blob/master/chinese/openwrt-pcduino/移植OpenWrt到pcDuino.md  
* https://openwrt.org/docs/guide-developer/packages  

## OpenWrt helloworld    
* https://openwrt.org/docs/guide-developer/helloworld/start  

## Linkit7688 OpenWrt  
* https://github.com/waynepiekarski/linkit-smart-7688-openwrt  
* https://github.com/MediaTek-Labs/linkit-smart-7688-feed  
* https://github.com/MediaTek-Labs/linkit-smart-7688-feed/blob/master/mtk-linkit/Makefile  
* https://github.com/brucepom/custom_linkit  

## 为联发科Linkit-Smart-7688编译openwrt的方法  
* http://etrd.org/2017/05/11/%E4%B8%BA%E8%81%94%E5%8F%91%E7%A7%91Linkit-Smart-7688%E7%BC%96%E8%AF%91openwrt%E7%9A%84%E6%96%B9%E6%B3%95/  

## spi-tft  
* https://github.com/MagicPrince666/spi-tft  

## i2c  
* https://github.com/RF-Networks/openwrt-RFN-feed/tree/master/i2c-tools  

## test1  
* https://github.com/lurancehuahua/test1  

## 司徒的教學網站  
* https://steward-fu.github.io/website/mcu.htm  
* https://steward-fu.github.io/website/mcu/smart_mt7688/framebuffer.htm  

## 无涯MT7688开发板  
* MT7688学习笔记（1）——搭建环境、编译烧写  
* https://blog.csdn.net/qq_36347513/article/details/81508385  
* https://blog.csdn.net/qq_36347513/article/details/81543094  
* https://gitee.com/hi-wooya/projects  
* https://github.com/hi-wooya?tab=repositories  
* search 无涯_mt7688, WKA-M76S_开发手册_V1.1_2021.09.28.pdf  

## VoCore2, MT7628, The Coin-sized Linux Computer    
* https://vocore.io/v2.html  
* Directly write to memory/register  
```
Directly write to memory/register
We made a simple tool for this, download here, its name is "mem", put the executable file into /bin/ in VoCore2.
1. read from register/memory, for example: 0x10000060, pin control register
example: mem 0x10000060
2. write to register/memory, must in 32bits(4bytes)
example: mem 0x10000064 0x05540555
here is an example bash script flash the LED every second on VoCore2
mem 0x10000064 0x05540555; 
mem 0x10000604 0x1000; 
while [ 1 ]; 
  do mem 0x10000634 0x1000; 
  sleep 1; 
  mem 0x10000644 0x1000; 
  sleep 1; 
done
```
* http://vonger.cn/misc/vocore2/tools/mem.zip  
* https://www.bilibili.com/video/av17827335  


## 智能路由器开发指南  
(baidupan) pdf  

## mt7688  
https://github.com/KianWeng/mtk7688  

## Lean's OpenWrt source  
https://github.com/coolsnowwolf/lede  

## nanopi-openwrt  
https://github.com/klever1988/nanopi-openwrt  

## wrtnode  

## 7688hdk  
* https://mangopi.org/7688hdk
* MT7688_Datasheet_v1_4  

## qemu-mt7628  
* https://github.com/newluhux/qemu-mt7628  

## 使用MT7688A的SPI驱动液晶屏（framebuffer方式）WIDORA NEO   
* https://www.amobbs.com/thread-5686620-1-1.html  
* python内核 7688_使用MT7688A的SPI驱动液晶屏（framebuffer方式）WIDORA NEO  
* https://blog.csdn.net/weixin_35143166/article/details/113970298
* https://mangopi.org/7688hdk
* SPI驱动液晶屏（framebuffer方式）
* https://mangopi.org/7688dev  
* https://mangopi.org/ips
* (NOT MT7688) 使用 LicheeRV 86 Panel 与 Tina BSP 实现 RGB 与 SPI 双屏显示  
* https://wiki.sipeed.com/soft/Lichee/zh/Lichee-RV/contribution/Dual_screen_display/Dual_screen_display.html  
* (NOT MT7688) luckfox, SPI 驱动 LCD  
* https://wiki.luckfox.com/zh/Luckfox-Pico/Luckfox-Pico-LCD/  

## vocore2 screen  
* https://vocore.io/screen.html  
* set screen to black: dd if=/dev/zero of=/dev/fb0 bs=1000 count=768  
* set screen to random pixel: dd if=/dev/urandom of=/dev/fb0 bs=1000 count=768
* some tuturial, not good, see https://v.youku.com/v_show/id_XNDE0Mzk1MjUyOA==.html  
```
ckermit
cd /mnt/mmcblk0p1/
ls
insmod fbusb.vocore2.ko
(connect screen)
dd if=/dev/zero of=/dev/fb0 bs=1024 count=768
dmesg > /dev/tty
dmesg > /dev/tty0
./xdoom.vocore2
dd if=/dev/zero of=/dev/fb0 bs=854 count=480
```
* source see :  
https://github.com/Vonger/vocore2  
https://github.com/Vonger/vocore2/tree/master/utils  
https://github.com/Vonger/vocore2/tree/master/utils/fbusb  
https://github.com/Vonger/vocore2/tree/master/utils/lvgl-fb-demo  
https://github.com/Vonger/vocore2/tree/master/utils/libsdl  
* How to run vocore2 lvgl firmware rom    
see https://github.com/weimingtom/wmt_lvgl_study/blob/master/README.md  
see http://vonger.cn/misc/screen/20200927.bin.xz  
see https://vocore.io/v2u.html  
see https://vonger.cn/misc/screen/  
see https://vonger.cn/misc/screen/20200628.touch.bin.xz
```
我搞明白怎么用vocore2运行LVGL例子和驱动usb屏幕，
之前失败其实是因为fbusb.ko的驱动程序不兼容（因为需要和内核版本完全一样才能正确运行），
所以要么重新编译内核或者重新编译驱动程序。
然后我想起其实可以通过wifi来刷固件，然后找了一下，发现有个touch固件自带fbusb驱动和LVGL，
刷完就可以看到LVGL例子（开机启动，不需要insmod）。具体效果略，
因为触摸比较卡顿，可能和屏幕速度或者mt7628主频低有关，也许作者不想明说
```  
```
1. use PC wireless connect to your VoCore hotspot, open browser view 192.168.1.1 or 192.168.61.1 (I use 61.1).  
2. LuCI console using username: root, password: vocore,  
3. select "System" -> "Backup/Flash Firmware"   
4. uncheck 'keep settting', and "Flash Image". choose 20200628.touch.bin  
5. after flashing, will auto start running /root/demo, it's a LVGL demo program  
```
