# OMIT

This is the meta-repository for the Open Mesh Infrastructure for Telemetry (OMIT) project. This repository contains

- Architectural Documents
- Reference Implementations
- Sample Code

The goal of OMIT is to provide an unstoppable, uncensored, worldwide messaging infrastructure on heterogeneous network layers including Internet, Short Wave/VHF/UHF radio, LoRaWAN, WiFi and Bluetooth


![](https://raw.githubusercontent.com/romeokienzler/omit/master/images/%20reference_architecture.png "")

## Example Deployment


![](https://raw.githubusercontent.com/romeokienzler/omit/master/images/example1.png "")

This tiny little example should give you an idea on how a OMIT deployment looks like. It uses APRS in most of the cases but is open to use other low layer messaging protocols as well (e.g. LoRaWan, ...)

As you can see in the image above three mobile stations are involved (Android Devices) - two are connected to each other via direct APRS links on PMR466 and one gets messages forwarded via BlueTooth from a nearby Smartphone.

This traffic is monitored via an RTL2832 Dongle connected to a Raspberry Pi. Note that this is therefore one-way connection only. The received messages are forwarded to subscribed LoRaWan devices, to the Internet and to a remote node through a CB Radio link. This is the farest reaching technology, especially when used on 12 Watts SSB and a noise resistant mode like JT65, FT8 or ROS.

