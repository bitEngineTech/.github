# Security policy

This policy applies to every repository in the bitEngineTech organization and to bitEngine Hub
firmware releases.

## Reporting a vulnerability

Please do **not** open a public issue for a security problem.

1. Use GitHub's private vulnerability reporting on the affected repository
   (*Security* tab → *Report a vulnerability*).
2. If that option is not available, open a plain issue titled "Security contact request" with no
   details, and we will reply with a private channel.

Please include the firmware version, how to reproduce the problem, and what impact you believe
it has. We will acknowledge the report, keep you informed of progress, and credit you in the
release notes if you wish.

## Scope

In scope: the ESP32-C5 firmware and web UI, the EFR32MG24 NCP configuration, the update and
signing mechanism, and the hub's network services (EZSP over TCP, OTBR REST API, web UI).

Problems in upstream components (ESP-IDF, OpenThread, Silicon Labs EmberZNet, Home Assistant,
ZHA, Zigbee2MQTT) should be reported to those projects; we will track and ship the fix on our
side.

## Supported versions

Security fixes are provided for the latest release of each firmware. Older releases are not
patched; update to the current release.

## Design notes relevant to security

- Official firmware images are signed and the hub verifies signatures before applying updates.
- The ESP32-C5 secure-boot and flash-encryption eFuses are deliberately **not** burned, so owners
  can run their own firmware. This is a conscious trade-off in favour of user freedom; if you
  need a locked-down device, this product is not designed to be one.
- The hub's services (EZSP over TCP, OTBR REST API, web UI) are meant for a trusted LAN. Do not
  expose them to the internet; use a VPN if you need remote access.
