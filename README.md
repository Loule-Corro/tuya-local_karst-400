[![hacs_badge](https://img.shields.io/badge/HACS-Custom-41BDF5.svg)](https://github.com/hacs/integration)
[![hacs_badge](https://img.shields.io/badge/HACS-make--all%2Ftuya--local-41BDF5.svg)](https://github.com/make-all/tuya-local)

## Tuya Local Integration file for solar inverter Karst-400 (based on WVC-400) 

Based on the custom integration [make-all/tuya-local](https://github.com/make-all/tuya-local)

YAML file for Karst-400 solar inverter integration in Home Assitant, initially for the Avidsen Soria 400W solar Kit

## Installation

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge)](https://github.com/hacs/integration)

Copy the file in the homeassistant/custom_components/tuya_local/devices/ folder before reloading.

Now you can follow the steps at https://github.com/make-all/tuya-local?tab=readme-ov-file#configuration to add a new device. It seems that only 3.4 version of protocol is working with this device.

At step Two, you should be able to select Karst-400 type of device.

## Customisation

This YAML file is a template that you can modify to your needs. The mapping when you add a device is done with DPs (data points) match so you may need to adapt for other devices.

For those interested for the data points list, this si what is returned by Tuya Cloud:
```
{
  "result": {
    "properties": [
      {
        "code": "reverse_energy_total",
        "custom_name": "",
        "dp_id": 2,
        "value": integer
      },
      {
        "code": "pv1_dc_data",
        "custom_name": "",
        "dp_id": 3,
        "value": string
      },
      {
        "code": "phase_a",
        "custom_name": "",
        "dp_id": 7,
        "value": string
      },
      {
        "code": "power_total",
        "custom_name": "",
        "dp_id": 10,
        "value": integer
      },
      {
        "code": "fault",
        "custom_name": "",
        "dp_id": 11,
        "value": integer
      },
      {
        "code": "work_mode",
        "custom_name": "",
        "dp_id": 12,
        "value": string
      },
      {
        "code": "inverter_alarmset_1",
        "custom_name": "",
        "dp_id": 13
      },
      {
        "code": "inverter_alarmset_2",
        "custom_name": "",
        "dp_id": 14
      },
      {
        "code": "inverter_type",
        "custom_name": "",
        "dp_id": 15,
        "value": "Karst-400"
      },
      {
        "code": "inverter_id",
        "custom_name": "",
        "dp_id": 16,
        "value": string
      },
      {
        "code": "imei_imsi",
        "custom_name": "",
        "dp_id": 17,
        "value": string
      },
      {
        "code": "temp_current",
        "custom_name": "",
        "dp_id": 18,
        "value": integer
      },
      {
        "code": "switch",
        "custom_name": "",
        "dp_id": 101,
        "value": true
      },
      {
        "code": "pv_power",
        "custom_name": "",
        "dp_id": 102,
        "time": 1714654838510,
        "value": 334
      },
      {
        "code": "ac_power",
        "custom_name": "",
        "dp_id": 103,
        "value": integer
      },
      {
        "code": "energy_clear",
        "custom_name": "",
        "dp_id": 104,
        "value": "0"
      },
      {
        "code": "power_adj",
        "custom_name": "",
        "dp_id": 105,
        "value": 100
      }
    ]
  },
```

## Next

I will probably add more DPs and sensors later, the YAML files will be available here. Feel free to fork or share your work with a request.

## Thanks
You can support [make-all/tuya-local](https://github.com/make-all/tuya-local) for the great integration.


If you don't know what to do with your money, there are a lot of labs things waiting to be tested...

[![BuyMeCoffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/loule_c)
