This is a progress document for Hackintosh Ventura on model Acer Nitro 5 AN515-51

**Attempt 1**
* Downloaded and created Ventura installer with new & updated EFI
* Installed Ventura, but with no full compatibility (Wifi Card Unsupported, can't use iServices)
* Used a Wifi dongle with outdated software, so I installed chris111's WIfi USB Dongle software after it asking to turn off SIP.
* After installing, rebooting into Ventura immedieatly kernel panics, couldn't figure out why.

[FAIL]

My best bet to get this hackintosh to work is replace the Wifi card for iServices.

**Attempt 2**
[July 11th-12th] 
* New Wifi card arrives, installed into my laptop replacing Qualcomm Atheros unsupported card.
* Used my other hackintosh to install Ventura Beta app and create a new install media.
* Recreated EFI with updated kexts, installer boots up normally.
* Installed successfully with no issues.
* Tested everything.

| What was tested | Does it Work?                                                  |
| ------------------- | ------------------------------------------- |
| Wifi | Yes |
| Graphics & Hardware Acceleration | Yes, using integrated |
| Sound | Yes |
| Bluetooth | Unfortunately, not yet |
| iCloud & Services | Yes |
| Keyboard and trackpad | Yes, no delay |

Update: Bluetooth seems to not work because either BlueToolFixup.kext and/or IntelBluetoothFirmware.kext isn't working properly.

To conclude, this attempt was kinda successful. The only thing not working is Bluetooth, but everything else seems to be fine. Since this is a beta, I wouldn't expect everything to work right off. So when Ventura actually gets a stable release, it would be better to do it as everything gets updated.

[SUCCESS, KINDA]

(This will change in the future)
