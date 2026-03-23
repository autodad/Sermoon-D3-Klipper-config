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
  LCD screen

## Manual config requirements
```yaml
  [bltouch]
    z_offset: 2.50 # +/-0.25
```

  Commit to bed mesh config in file

## Things to remember before printing
  Calibrate heating elements PID
  
### Extruder
  `PID_CALIBRATE HEATER=extruder TARGET=210`
  Where TARGET is the temperature you usually use for your filament
### Build plate
  `PID_CALIBRATE HEATER=heater_bed TARGET=60`
  Where TARGET is the temperature you usually use for your bed
### Save
  There is no autosave so don't forget
  `SAVE_CONFIG`
