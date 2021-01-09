# compiled Linux kernel(s) 5.10.x for Lenovo Ideapad Flex-5 (AMD Ryzen 5)

* Finally 100% working linux kernel for IdeaPad Flex 5 series convertible laptops, versions with AMD Ryzen 5 (4000 series) CPU and chipset.
* 5.10 is going to be LTS kernel

## 5.10.5-xanmod

* applied patch for bluetooth
* [Xanmod](https://xanmod.org/) kernel is ubuntu/debian kernel tuned more toward desktop/laptop average user or their lowlatency versions 
are suitable for Linux gaming compared to stock kernel which is tuned rather for stability to be used by server users 
and enterprise sector too.
* original kernel source tarball: [https://github.com/xanmod/linux/archive/5.10.5-xanmod2-cacule.tar.gz](https://github.com/xanmod/linux/archive/5.10.5-xanmod2-cacule.tar.gz)

**important note after install** I observed that default actions for suspend/hibernation/hybrid sleep in XFCE desktop enviroment stopped
 working on this kernel, but hopefully to resolve this issue just reinstalation of **pm-utils** was enough.
```
sudo apt-get install --reinstall pm-utils
```

## 5.10 

* only bluetooth didn't worked - solved by patch*
* source from ubuntu kernel mainline PPA [ver. 5.10](https://kernel.ubuntu.com/~kernel-ppa/mainline/v5.10/)

## previous kernels used on this machine & issues

**5.9.x**
* bluetooth not working (solved by patch*)
* touchscreen and stylus not working

**5.8.x**
* sound card not 100% working - not able to switch default microphone, in some apps (google meet, zoom) microphone not detected
* thermal and fan speeds management not great

## install

Install in order:

* libc (maybe unnecessary)
* linux-headers
* linux-image

## credits

[Edward Vear (edwardvear@gmail.com)](https://marc.info/?l=linux-bluetooth&m=160378222632366&w=2)  
[Christian Britz (cbritz@t-online.de) at debian bugreports lists](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=972968)



