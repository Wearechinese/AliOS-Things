## Contents

## Introduction
supported boards' code here. It includes board init related codes.
    * board init codes
    * kernel config codes
    * startup.c which include main function
    * ld\scatter file
    * peripheral drivers for this board

### Features
- board supported

### Standand directories layout
```sh
|--board
    |--xxx
        |--config
        |   --board.h                   : board config file, define for user, such as uart port num             Y
        |   --k_config.c                : user's kernel hook and mm memory region define                        Y
        |   --k_config.h                : kernel config file .h                                                 Y
        |   --partition_conf.c          : board flash config file                                               N
        |--drivers                      : board peripheral driver                                               N
        |--startup
        |   --board.c                   : board config implement                                                Y
        |   --startup.c                 : main entry file                                                       Y
        |--xxx.ld                       : link script                                                           Y
        |--aos.mk                       : board makefile                                                        Y
        |--README
```
### Supported Boards
Aaboard_demo is a board demo for consuling, not a true realization.
* ARM
    * Cortex-M0
        * [eml3047](./eml3047/README.md)
        * [frdmkl26z](./frdmkl26z/README.md)
        * [frdmkl27z](./frdmkl27z/README.md)
        * [frdmkl28z](./frdmkl28z/README.md)
        * [frdmkl43z](./frdmkl43z/README.md)
        * [frdmkl81z](./frdmkl81z/README.md)
        * [frdmkl82z](./frdmkl82z/README.md)
    * Cortex-M3
        * [mk1101](./mk1101/README.md)
    * Cortex-M4
        * [amebaz_dev](./amebaz_dev/README.md)
        * [atsame54-xpro](./atsame54-xpro/README.md)
        * [b_l475e](./b_l475e/README.md)
        * [cy8ckit-062](./cy8ckit-062/README.md)
        * [cy8ckit-149](./cy8ckit-149/README.md)
        * [developerkit](./developerkit/README.md)
        * [gd32f4xx](./gd32f4xx/README.md)
        * [lpcxpresso54102](./lpcxpresso54102/README.md)
        * [lpcxpresso54608](./lpcxpresso54608/README.md)
        * [lpcxpresso54628](./lpcxpresso54628/README.md)
        * [lpcxpresso54114](./lpcxpresso54114/README.md)
        * [lpcxpresso54018](./lpcxpresso54018/README.md)
        * [mk3080](./mk3080/README.md)
        * [mk3165](./mk3165/README.md)
        * [mk3166](./mk3166/README.md)
        * [mk3239](./mk3239/README.md)
        * [pca10040](./pca10040/README.md)
        * [pca10056](./pca10056/README.md)
        * [starterkit](./starterkit/README.md)
        * [stm32f429zi-nucleo](./stm32f429zi-nucleo/README.md)
        * [stm32l432kc-nucleo](./stm32l432kc-nucleo/README.md)
        * [stm32l433rc-nucleo](./stm32l433rc-nucleo/README.md)
        * [stm32l476rg-nucleo](./stm32l476rg-nucleo/README.md)
        * [stm32l496g-discovery](./stm32l496g-discovery/README.md)
        * [uno-91h](./uno-91h/README.md)
        * [xr871evb](./xr871evb/README.md)
    * Cortex-M7
        * [stm32f769i-discovery](./stm32f769i-discovery/README.md)
        * [evkbimxrt1050](./evkbimxrt1050/README.md)
        * [evkmimxrt1020](./evkmimxrt1020/README.md)
    * ARM968E-S
        * [bk7231devkitc](./bk7231devkitc/README.md)
        * [bk7231udevkitc](./bk7231udevkitc/README.md)
        * [mk3060](./mk3060/README.md)
        *
* xtensa
    * [esp32devkitc](./esp32devkitc/README.md)
    * [esp8266](./esp8266/README.md)
* MIPS
    * MIPS-I
        * [rda8955](./rda8955/README.md)
* C-Sky
    * CK802
        * [cb2210](./cb2210/README.md)

### Dependencies

## Reference