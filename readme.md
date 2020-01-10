# RFM69 driver for ESP Open RTOS

This repository contains a port of André Heßling's [STM32 RFM69 driver](https://github.com/ahessling/RFM69-STM32) for the ESP8266. The included demo program sends the string "Hello World" over the air over and over again. RX has been tested also.

```
git clone https://github.com/kanflo/eor-rfm69 esp-open-rtos/extras/rfm69
git clone --recursive https://github.com/SuperHouse/esp-open-rtos.git
# Set wifi credentials
nano esp-open-rtos/include/ssid_config.h
cd rfm69/example
export EOR_ROOT=$PWD/../../esp-open-rtos
make && make flash
```
