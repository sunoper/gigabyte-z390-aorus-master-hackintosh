# Hackintosh Catalina Installation Guide for Gigabyte Z390 Pro wifi

This build is "Vanilla". I used [this guide](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/) as a starting point.

I assume you are installing Catalina, although most of the instructions also apply for Mojave.

### Hardware

See my [Hardware List](HARDWARE.md)

![About My Mac](images/about.png)

### What's Working/What's Not

##### Working
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
- Bluetooth & Wi-Fi (via Broadcom adapter. Also works in UEFI and Clover.)
- Unlock with Apple Watch
- Airdrop
- AirPlay
- Continuity
- Apple Music (iTunes)
- DRM-protected videos in TV app (not working in Mojave)
- Power Nap


##### Not Working
- Built-in wifi. This will likely never work since it is the new Intel CNVi that MacOS doesn't support.
- Onboard Bluetooth is hit or miss. However, I disabled it (HS14) because I have a natively supported Broadcom BCM94360CS2 WIFI/BT adapter.
- Netflix DRM in Safari (works in Chrome)


##### Not Yet Tested
- FileVault


### Step By Step Instructions

See [STEP_BY_STEP.md](STEP_BY_STEP.md)

### USB Port Map & SSDT

See [USB_MAP.md](USB_MAP.md) for a map of all the ports on the Aorus z390 Master.

### The Lazy Way

You are welcome to use my config.plist and kexts. However, make sure you set the following:

- SerialNumber
- BoardSerialNumber
- SmUUID
