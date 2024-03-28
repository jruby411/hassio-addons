# Home Assistant Add-on: AWNET

Local data transfer between Ambient Weather weather station and Home Assistant.

## About

You can use this add-on to take advantage of the new "Custom Server" feature in AWNET available in Firmware [4.2.8](https://ambientweather.com/support) on the WS-2902A, WS-2902B, WS-2902C, WS-2000 And WS-5000. I have tested this using my WS-2902C. It presents a webserver that will accept the polling from the WS device. It then calls a service provided by the [Ambient Weather Station - Local](https://github.com/tlskinneriv/awnet_local) custom integration to ingest data.

This add-on and integration combo are a work in progress. Any feedback and/or contributions are appreciated. Credit to [dancwilliams](https://github.com/dancwilliams) for the [initial add-on](https://github.com/dancwilliams/hassio-addons/tree/master/awnet) that this was forked from.

## Changes by jruby411

I added a couple of tweaks to what tlskinneriv has done. I orginally ran Home Assistant core in a docker container and had to configure and build this Add-on as a stand-alone container. You can find this earlier work on [gitlab](https://gitlab.com/jruby411/awnet). It was an eperiment in many ways. I decided to start over with my Home Assistant and I now run a supervised version on Debian 11 in a Proxmox VM. This is now my firt experience in to "hassio supervised" Add-ons.

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg
