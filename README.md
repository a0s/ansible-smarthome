SmartHome
=========

I extend the life of my old refrigerator with [Home Assistant](https://www.home-assistant.io/) and smart plug. 

<img width="487" alt="Temperature diagram" src="https://user-images.githubusercontent.com/418868/85892494-b636b600-b7f9-11ea-947e-50f880aa8de2.png">


Hardware
--------

* [Cubieboard2](http://cubieboard.org/model/cb2/) with the latest Armbian
* [TP-Link HS110 smart plug](https://www.tp-link.com/uk/home-networking/smart-plug/hs110/)
* [Xiaomi WSDCGQ11LM temperature sensor](https://www.aliexpress.com/i/32974302289.html)
* [RTL8192CU WiFi USB dongle](https://www.aliexpress.com/item/32859398234.html) 
* [CC2531 ZigBee USB dongle](https://www.aliexpress.com/item/4000028865267.html)

Installation
------------

```shell script
ansible-galaxy install -r requirements.yml
ansible-playbook -i inventories/smarthome playbooks/smarthome.yml
```

Environments
------------

* `SMARTHOME_PRIVATE_WIFI_SSID` - wifi ssid
* `SMARTHOME_PRIVATE_WIFI_PASSWORD` - wifi password
