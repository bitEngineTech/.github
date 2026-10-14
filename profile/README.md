# bitEngine

Open smart home hardware, built for Home Assistant.

## bitEngine Hub

A PoE-powered gateway that runs **Zigbee 3.0 and Thread at the same time on two independent
radios**, with Ethernet / 802.3af PoE and a 5 GHz Wi-Fi 6 fallback uplink. One cable, placed where
the RF coverage is best. The Thread border router runs on the device, so no add-on is needed in
Home Assistant; the Zigbee coordinator is exposed as standard EZSP over TCP for ZHA and
Zigbee2MQTT.

- Product page and newsletter: <https://home.bitengine.tech>
- Dev-log and feedback thread: [Home Assistant Community forum](https://community.home-assistant.io/t/1028644)
- Crowd Supply campaign: target launch December 2026

| Repository | What it holds | License |
|---|---|---|
| [bitengine-hub-firmware](https://github.com/bitEngineTech/bitengine-hub-firmware) | ESP32-C5 application firmware and embedded web UI; Home Assistant integration docs | Apache-2.0 |
| [bitengine-hub-zigbee-ncp](https://github.com/bitEngineTech/bitengine-hub-zigbee-ncp) | EFR32MG24 Zigbee NCP: Simplicity Studio project, bootloader, release images | Apache-2.0 (images: Silicon Labs MSLA) |
| [bitengine-hub-hardware](https://github.com/bitEngineTech/bitengine-hub-hardware) | Schematics, 3D-printable enclosure, mechanical documentation | CERN-OHL-P-2.0 |
| [bitengine-home-site](https://github.com/bitEngineTech/bitengine-home-site) | Source of home.bitengine.tech | — |

**Where things stand (October 2026):** hardware and firmware are working on prototype units;
tested with Home Assistant ZHA, Zigbee2MQTT validation in progress. Firmware source is scheduled
for release in **November 2026**, schematics at the campaign launch. FCC and CE certification are
planned for the production design.

## Contributing and security

Issues and pull requests are welcome in the repository they concern — see
[CONTRIBUTING](https://github.com/bitEngineTech/.github/blob/main/CONTRIBUTING.md).
For security issues, please read [SECURITY](https://github.com/bitEngineTech/.github/blob/main/SECURITY.md)
before posting anything public.
