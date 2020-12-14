# compiled Linux kernel 5.10 for Lenovo Ideapad Flex-5 (AMD Ryzen 5)

* Finally 100% working linux kernel for IdeaPad Flex 5 series convertible laptops, versions with AMD Ryzen 5 (4000 series) CPU and chipset.
* 5.10 is going to be LTS kernel
* source from ubuntu kernel mainline PPA [ver. 5.10](https://kernel.ubuntu.com/~kernel-ppa/mainline/v5.10/)

## kernels & issues

**5.10**
* only bluetooth didn't worked - solved by patch*

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



