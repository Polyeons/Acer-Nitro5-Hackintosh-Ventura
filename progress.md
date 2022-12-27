This is a progress document for Hackintosh Ventura on model Acer Nitro 5 AN515-51

**Attempt 1**
* Downloaded and created Ventura installer with new & updated EFI
* Installed Ventura, but with no full compatibility (Wifi Card Unsupported, can't use iServices)
* Used a Wifi dongle with outdated software, so I installed chris111's WIfi USB Dongle software after it asking to turn off SIP.
* After installing, rebooting into Ventura immedieatly kernel panics, couldn't figure out why, didn't really look into it.

[FAIL]

The owner of the repository I forked from was using a Wifi dongle for his build, as was I. 
I ordered a replacement Wifi card. (Intel AC-7265 Dual-Band)

**Attempt 2**
[July 11th-12th] 
* New Wifi card arrives, installed into my laptop replacing the Qualcomm Atheros card, which was unsupported resulting to use a USB wireless reciever.
* Used my other hackintosh to install Ventura Beta app and create a new install media.
* Recreated EFI with updated kexts, installer boots up normally.
* Installed successfully with no issues.
* Tested everything.

| What was tested | Does it Work?                                                  |
| ------------------- | ------------------------------------------- |
| Wifi | Yes |
| Graphics & Hardware Acceleration | Yes, using integrated |
| Sound | Yes |
| Bluetooth | Yes |
| iCloud & Services | Yes |
| Keyboard and trackpad | Yes, no delay |

Any features introduced in Ventura do work, with some exceptions. Continuity Camera (use an iPhone as webcam) does not work unless you use a supported Broadcom card. Maybe in the future with an offical or communuity made kext.

Another update: Looks like I was wrong, whoops! Bluetooth is working now after adding SSDT-USB-RESET and it reads as normal now, finally!

To conclude, this attempt was a success. The only thing not working was Bluetooth, but now everything seems to be fine. Because this is a beta, I wouldn't expect everything to work. Better to wait for Apple to release Ventura. 

(This will change in the future)
