# Hackintosh for Asrock B365 itx/ac via OpenCore

This is mainly here for my benefit more than anyone elses, but you're welcome to
use or modify these files in any way if you believe they can be of assistance to
you.

<!-- However, make sure you set the following:

- SystemSerialNumber
- SystemUUID
- MLB -->

## Version

| Type     | Version |
| :------- | :------ |
| OpenCore | 0.7.8   |
| MacOS    | 11.6.3  |

## Hardware

| Type            | Item                         |
| :-------------- | :--------------------------- |
| **CPU**         | Intel Core i5-8400           |
| **Motherboard** | ASRock B365M-ITX/ac Mini ITX |
| **Video Card**  | Radeon RX 580 8 GB           |
| **Wifi card**   | Broadcom Bcm943602cs         |

## Functionality

### Works

- Ethernet
- Onboard Audio (including digital audio)
- APFS
- Sleep/Wake
- All USB ports at 3.x speed
- iMessage
- App Store
- Facetime
- APFS
- Handoff
- Bluetooth & Wi-Fi
- Airdrop
- AirPlay
- Continuity
- Power Nap
- NVRAM
- Igpu headless mode (must be headless mode if you want Airplay works)
- Wired Sidecar

### Doesn't work

- Onboard Wifi: Won't work, I removed it and replaced with Broadcom Bcm943602cs Card
- Wireless Sidecar

### Not Yet Tested

- FileVault
- All DRMs:
  - iTunes Movies (FairPlay 1.x)
  - Netflix (FairPlay 2.x/3.x)
  - Some Amazon Prime content, but not all. (FairPlay 2.x/3.x)
  - Apple TV+ (FairPlay 4.x)

## Instructions

[OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/).

When you have troubles, take look at my kexts, drivers, ACPI and config.list for help.

## SSDT

| SSDT             | Usage                  |
| :--------------- | :--------------------- |
| SSDT-EC-USBX.aml | EC                     |
| SSDT-PLUG.aml    |                        |
| SSDT-PMC.aml     |                        |
| SSDT-USBX.aml    | EC                     |
| SSDT-UIAC.aml    | with USBInjectAll.kext |

## USB Port Map

I will update later if I have time.
