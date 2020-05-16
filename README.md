# Hackintosh for Asrock B365 itx/ac via OpenCore

<p align="center">
  <img src="https://i.imgur.com/1lqffJF.png" alt="About this mac specs">
</p>

> Attention: I'm no longer using the Asrock B365 itx so this is the last time I update this EFI.
> But I believe this EFI config is still helpful for whom started with this mainboard.
> If you have any questions, please leave it at `issues`.

This is mainly here for my benefit more than anyone elses, but you're welcome to use or modify these files in any way if you believe    they can be of assistance to you.

However, make sure you set the following:

- SystemSerialNumber
- SystemUUID
- MLB


## Hardware

Type|Item
:----|:----
**CPU** | [Intel Core i5-9400 2.9 GHz 6-Core Processor](https://pcpartpicker.com/product/V4RzK8/intel-core-i5-9400-29-ghz-6-core-processor-bx80684i59400)
**Motherboard** | [ASRock B365M-ITX/ac Mini ITX LGA1151 Motherboard](https://pcpartpicker.com/product/4DBTwP/asrock-b365m-itxac-mini-itx-lga1151-motherboard-b365m-itxac)
**Video Card** | [Gigabyte Radeon RX 580 8 GB Gaming 8G Video Card](https://pcpartpicker.com/product/KQQRsY/gigabyte-radeon-rx-580-8gb-gaming-8g-video-card-gv-rx580gaming-8gd)

## What work and what doesn't

### Works:
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
- Bluetooth & Wi-Fi (via Broadcom adapter)
- Airdrop
- AirPlay
- Continuity
- ALL DRMs:
  - iTunes Movies (FairPlay 1.x)
  - Netflix (FairPlay 2.x/3.x)
  - Some Amazon Prime content, but not all. (FairPlay 2.x/3.x)
  - Apple TV+ (FairPlay 4.x)
- Power Nap
- NVRAM
- IGPU: you can switch to branch `igpu` to use IGPU


### Doesn't work:

* Onboard Wifi: Won't work, I removed it and replaced with DW1560 Broadcom BCM94352Z Card
* Sidecar: I don't have Ipad to test.

### Not Yet Tested

- FileVault

## Step By Step Instructions

I literally just followed the [OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/). When you have troubles, take look at my KEXTs, drivers and config.list for guidance.


## USB Port Map & SSDT

I will update later if I have time.
