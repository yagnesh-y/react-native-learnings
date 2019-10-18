# react-native-learnings
Learnings and notes on cross platform apps development using ReactNative


#### Debugging release app:
    Android: Release apk on device -> connect device -> check for adb logs(adb logcat *:S ReactNative:V ReactNativeJS:V)
    iOS: Relase ipa on device -> connect device -> check for logs in xCode(open debug console CMD+SHIFT+C)
    

#### Changing appName:
Say you've given some appName and later need to change the appName without modifying the bundle/package id as we dont wan't to setup all the native modules again.
     
     Android: Change the app_name value in strings.xml file
     iOS: Change the Bundle Display Name value in the info.plist file
