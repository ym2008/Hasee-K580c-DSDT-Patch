# Hasee-K580c-DSDT-Patch

This branch for BCM94352HMB.

What works: 

+ CPU: Intel Core i7-4700MQ

+ Chipset: Intel HM86 Chipset

+ Wifi: Broadcom BCM94352HMB

+ Lan: Realtek RTL8168G/8111G

+ Audio: Realtek ALC282

+ Integrated Graphics: Intel HD Graphics 4600 1536 MB

+ Bluetooth: Broadcom BCM20702A0

+ Card Reader: Realtek PCIE CardReader

+ Webcam: USB HD Webcam

+ HDMI: Video + Audio

+ USB 2.0 / 3.0

+ FN Keys 

+ Touchpad with gestures

+ Brightness slider

+ Battery status

+ Sleep / Wake

+ Speedstep

What does not work:

- Dedicated graphics: NVIDIA Geforce GT750M (Disabled in Hotpatch)


All update for 10.13.3, such as APFS.efi.

Notes: 
	
	Please using Eject RTSX to eject SD Card.

By the way, I disable TRIM for SSD by default. If you want to enable it, you can change the disabled of the Enable TRIM for SSD to No. And add abm\_firstpolldelay=8000 in config.plist / Boot / Arguments. (For example, to set FirstPollDelay to 16000 (16 seconds), use abm_firstpolldelay=16000)

I set brcmfx-country=HK in config.plist / Boot / Arguments, if you want to change it, you can change HK to what the country you want, such like CN, US etc.

If you meet the brightness can not adjust, please rebuild cache and repair permissions. (e.g. Kext Utility)

If you hear a murmurs when pressing the Caps Lock, you can replace ApplePS2SmartTouchPad.kext with VoodooPS2Controller.kext.


+ You can try this repository on TWJ/TWK/TWS Model.