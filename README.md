iTransmission
==========
iTransmission is a torrent app for iOS (iPhone and iPad) which uses libtransmission for a backend.

So, what is iTransmission 4? iTransmission , originally, was developed by [ccp0101](https://github.com/ccp0101). It is no longer kept active. The previous

**UPDATE 2018-05-15:** This is a fork of a fork of a project, that appears to have some incredibly unpleasant and outright broken dependencies. It will not currently compile. I am attempting to refactor or rebuild using this as inspiration; watch this space for changes.

How to compile libraries
-----
Open terminal
cd to Compilation directory
./build.sh
If you need to change options, edit the configuration & build.sh file in Compilation directory. 

Compiling app
-----
1. The app will never be accepted in the app store. Therefore, we do not need codesigning. But XCode requires us to codesign each and every app. Assuming you use the iOS 9.3 SDK, I can disable this check by opening /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS9.3.sdk/SDKSettings.plist with a text editor and change the following values 

```
<key>CODE_SIGNING_REQUIRED</key>
<string>YES</string>
```
to 
```
<key>CODE_SIGNING_REQUIRED</key>
<string>NO</string>
```


```
<key>ENTITLEMENTS_REQUIRED</key>
<string>YES</string>
```
to 
```
<key>ENTITLEMENTS_REQUIRED</key>
<string>NO</string>
```

2. Alternatively, sign up for a free Apple Developer account, and sign into Xcode; Xcode will manage codesigning for you.

Installation
-----
1. Xcode will deploy the IPA to a device attached to the computer configured for development.

2. Manually install the IPA build product via iTunes or Configurator or iMazing, etc.

Credits
-------
- [Transmission](http://www.transmissionbt.com/)
- [ccp0101](https://github.com/ccp0101)
- [ioshomebrew](https://github.com/ioshomebrew)
- [fopino](https://github.com/fopino)
- [heavenly-awker](https://github.com/heavenly-awker)
- [Bilibili](https://github.com/Bilibili/ijkplayer)
- [Friend-LGA](https://github.com/Friend-LGA/LGSideMenuController)

Mail me if I missed somebody.
