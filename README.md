# react-native-learnings
Learnings and notes on cross platform apps development using ReactNative


#### Debugging release or debug app:
    Android: Release apk on device -> connect device -> check for adb logs(adb logcat *:S ReactNative:V ReactNativeJS:V)
    iOS: Relase ipa on device -> connect device -> check for logs in xCode(open debug console CMD+SHIFT+C)
    

#### Changing appName:
Say you've given some appName and later need to change the appName without modifying the bundle/package id as we dont wan't to setup all the native modules again.
     
     Android: Change the app_name value in strings.xml file
     iOS: Change the Bundle Display Name value in the info.plist file

#### Failure linking native modules:
Follow the debugging guide and watch out for the logs as they will let you know where the issue might be.

#### Some handy commands:

    Want to run app on a connected device: 
        Android: Connect device to system -> Enable debugging -> react-native run-android --deviceId XYX(using adb device to get list of deviceId's)
        iOS: Conect device to system -> Enable debugging -> react-native run-ios --device “Device name”(check for deviceName in your device settings)
        
     Open debugging menu from cmd line without shaking gesture
           
