# Tasmota Build - Preconfigured Tasmota IoT firmware for specific Module

[![tasmota-build-release](https://img.shields.io/github/v/release/racksync/tasmota-build)](https://github.com/racksync/tasmota-build) [![last commit](https://img.shields.io/github/last-commit/racksync/tasmota-build)](https://github.com/racksync/tasmota-build)

## What's Tasmota?

Tasmota easily integrates with many home automation solutions reporting status and sensor data and allowing complete control. Tasmota contains myriad features and supported peripherals (sensors, controllers and similar). Due to the flash size and memory constraints of ESP not all features can be included in precompiled release binaries.

To enable some of the features you have to compile your own binary. Features with such requirement have a warning with instructions on how to enable them.

## Original Problem

Tasmota firmware comes with many configurable parameters that are not set to proper value by default. We have compiled all necessary parameters to make it easier for you to use and reduce setup time for each modules type.


## Preconfigured Parameters List

- Change different config holder to avoid parameter conflict 
- Use uppercase as project name 
- Specific Module for each device
- Avoid default module reset (incase of factory reset)  
- Correct GPIO template for none module device 
- Enable mDNS by default 
- Provide access to webserver by  ```hostname.local``` 
- Reduce teleperiod time to ```10s``` 
- Setup default MQTT Host to mostly use as ```homeassistant.local``` 
- Specific Timezone for UTC+7 
- Enable LED Status as POWER 
- Disable fast power cycle detection for device reset by power failure issue
- Relay power on state as ```off``` 
- Enable factory reset by button (Most first button or GPIO0) 
- Change Webserver port to another 
- Enable Web Authentication 



## Preconfigured Module

Choose the right method for each module that matches your device model.


| Module                    | Serial Flash                          | OTA Upgrade                            |
| ------------------------- | ------------------------------------- | ----------------------------------------   |
|  Sonoff 4CH               | ```sonoff_4ch.bin```                  | ```sonoff_4ch.bin.gz```                     |       
|  Sonoff 4CH Pro           | ```sonoff_4ch_pro.bin```              | ```sonoff_4ch_pro.bin.gz```                |  
|  Sonoff Basic             | ```sonoff_basic.bin```                | ```sonoff_basic.bin.gz```                  |  
|  Sonoff Mini R2           |   ```sonoff_mini.bin```               |     ```sonoff_mini.bin.gz```             |
|  Sonoff POW Origin (R316) | ```sonoff_pow_origin.factory.bin```   |    ```sonoff_pow_origin.bin```             |
|  Sonoff POW R3            | ```sonoff_pow_r3.bin```               |  ```sonoff_pow_r3.bin.gz```             |
|  Sonoff S31               |```sonoff_s31.bin```                   |  ```sonoff_s31.bin.gz```               |
|  Sonoff SV                | ```sonoff_sv.bin```                   |    ```sonoff_sv.bin.gz```                |
|  Sonoff TH (Original)     | ```sonoff_th.bin```                   |        ```sonoff_th.bin.gz```          |
|  Sonoff TX 1C             |  ```sonoff_tx_1c.bin```               |  ```sonoff_tx_1c.bin.gz```             |
|  Sonoff TX 2C             | ```sonoff_tx_2c.bin```                |    ```sonoff_tx_2c.bin.gz```                |
|  Sonoff TX 3C             |  ```sonoff_tx_3c.bin```               |     ```sonoff_tx_3c.bin.gz```               |
|  Sonoff M5 1C             |    ```sonoff_m5_1c.factory.bin```     | ```sonoff_m5_1c.bin```                     |
|  Sonoff M5 2C             | ```sonoff_m5_2c.factory.bin```        | ```sonoff_m5_2c.bin```                     |
|  Sonoff M5 3C             |  ```sonoff_m5_3c.factory.bin```       |      ```sonoff_m5_3c.bin```                |

## How to Over-the-Air Upgrade?

### ESP8266 OTA 

1. To prevent out-of-space issue, Upload the original ```tasmota-minimal.bin.gz``` via web upgrade once.
2. Upload desire firmware file (eg: ```sonoff_basic.bin```) then.

### ESP32 OTA

1. Upload the module firmware (eg: ```sonoff_pow_origin.bin```) via web upgrade to entering safe boot.
2. Upload that firmware again. 


<!-- ![racksync-screenshot](https://github.com/racksync/hass-addons-cloudflared-tunnel/blob/main/zerotrust/screenshot.png?raw=true) -->

### Links

- [Services & Products](http://racksync.com)
- [Training Course](https://facebook.com/racksync)

### Community

- [Home Automation Thailand](https://www.facebook.com/groups/hathailand)
- [Home Automation Marketplace](https://www.facebook.com/groups/hatmarketplace)
- [Home Automation Thailand Discord](https://discord.gg/Wc5CwnWkp4) 

## [RACKSYNC CO., LTD.](https://racksync.com)

We are an expert in Automation and Smart Solutions of all sizes. We provide consulting services as well as system implementation. Installed and monitored by experts We are also a full-service Software As A Service development company.
\
\
RACKSYNC COMPANY LIMITED \
Suratthani, Thailand  \
Email : devops@racksync.com \
Tel : +66 85 880 8885 

[![Home Automation Thailand Discord](https://img.shields.io/discord/986181205504438345?style=for-the-badge)](https://discord.gg/Wc5CwnWkp4) [![Github](https://img.shields.io/github/followers/racksync?style=for-the-badge)](https://github.com/racksync) 
[![WebsiteStatus](https://img.shields.io/website?down_color=grey&down_message=Offline&style=for-the-badge&up_color=green&up_message=Online&url=https%3A%2F%2Fracksync.com)](https://racksync.com)



