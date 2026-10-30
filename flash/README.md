# 烧录

## 首选：网站免费烧录

直接点 [switchc.shop 烧录页](https://switchc.shop/flash.html)，插上 ESP32-S2 mini，按住 0/BOOT 点 RST 后连接串口，点免费烧录即可。

## 进阶：esptool.py

```bash
python -m esptool --chip esp32s2 --port COMx --baud 115200 write_flash -z \
  0x1000 firmware/0.2.0/bootloader.bin \
  0x8000 firmware/0.2.0/partitions.bin \
  0xE000 firmware/0.2.0/boot_app0.bin \
  0x10000 firmware/0.2.0/switchc_app.bin
```

COMx 换成实际串口号。固件地址、大小与网站烧录页一致。
