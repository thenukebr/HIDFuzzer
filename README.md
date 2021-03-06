# HIDFuzzer
An android app that allows you to play around with emulating an HID device.

Requires https://github.com/pelya/android-keyboard-gadget patch applied to the kernel to expose `/dev/hidg0` and `/dev/hidg1`.

Use at your own risk.

A couple of demo applications are implemented:
- Fuzzing of HID protocol
- PowerShell download and run executable
- PowerShell download and run PowerShell script
- Serial transfer of data through output reports
- Change wallpaper ([video demonstration](https://my.mixtape.moe/zxerjz.mp4))
- Probably more but I was too lazy to update readme

For people who want to implement HID functionality in their own apps, HID is interfacing code available [here (HID.java)](https://github.com/Netdex/HIDFuzzer/blob/master/app/src/main/java/cf/netdex/hidfuzzer/hid/HID.java), 
and a simple ease-of-use wrapper is available [here (HIDR.java)](https://github.com/Netdex/HIDFuzzer/blob/master/app/src/main/java/cf/netdex/hidfuzzer/hid/HIDR.java). The documentation should be enough to understand how it works.

Requires ChainFire's [libsuperuser](https://github.com/Chainfire/libsuperuser) to keep a su shell open.

**Q:** Why is the app so ugly?<br>
**A:** :cry: (functionality over fashion)

<img src="https://my.mixtape.moe/ogkgoz.png" width=200/>
