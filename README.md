# AOS course material for concurrency and the embedded part

This repository has git submodule, after cloning it do:

```
$ git submodule init
$ git submodule update
```

To compile the Miosix examples, download the latest version of the compiler here

https://miosix.org/wiki/index.php?title=Miosix_Toolchain

then ```cd``` into an example directory and type ```make```.

If you have an STM32F407 discovery board you can connect it and flash it with ```make program```.

The serial port is connected to pins

* PB10 TX (connect to RX pin of an USB to serial adapter)
* PB11 RX (connect to TX pin of an USB to serial adapter)

The SPI port is connected to the following pins

* PB3 SCK
* PB4 MISO
* PB5 MOSI
* PB7 CS

The 01-linker-boot example for RISC-V is provided without a Makefile as the STM32F407 is actually an ARM microcontroller, not RISC-V.
