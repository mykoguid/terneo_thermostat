# Terneo Thermostat component for Home Assistant

![Validate](https://github.com/mykoguid/terneo_thermostat/workflows/Validate/badge.svg)

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/custom-components/hacs) 

**Required device firmware version 2.3 and higher**

In case you don't use HACS just put `terneo_thermostat` folder to the `custom_components`

### Config example:
Add your device to `configuration.yaml`:
```
climate:
  - platform: terneo_thermostat
    serial: 'DEVICE_SERIALNUMBER'
    host: 'DEVICE_IP'
```
Serial number can be found on the page  http://`{device_ip}`/index.html in device info section.

### Common problems:
* In firmware version 2.3, the ability to control the local network by default blocked for security reasons.
Block removing - https://terneo-api.readthedocs.io/ru/latest/en/safety.html

### Useful Links
* Terneo API: https://terneo-api.readthedocs.io/ru/latest/
