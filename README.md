### spi0-ili9341 DTB

SPI0 linux framebuffer DTB for Waveshare 2.4inch LCD dislay (2.4inch_LCD_Module) for Raspberry Pi.

### Usage:
1. Compile the dtbo
2. Copy over the generated dtbo to /boot/firmware/overlays
3. Use the overlay in config.txt to use the dtb (eg: ```dtoverlay=spi0-ili9341,rotate=0,speed=64000000,width=240,height=320```)


### Compiling DTBO:
```dtc -@ -I dts -O dtb -o spi0-ili9341.dtbo spi0-ili9341.dts```