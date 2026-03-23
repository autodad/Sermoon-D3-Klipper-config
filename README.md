# Sermoon-D3-Klipper-config
Klipper configuration for Creality Sermoon D3

## Settings for klipper make menuconfig
  Micro-controller Architecture: STMicroelectronics STM32
  Processor model: STM32F401
  Bootloader offset: 64KiB bootloader
  Communication interface: Serial (on USART1 PA10/PA9)

## Not Working:
  Camera
  Loadcell for automatic Z-Offset

## Manual config requirements
  [bltouch]
    z_offset: 2.50 +/-0.25
