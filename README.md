# OnePlus Nord Debloat List

This is a list of uninstall commands for preinstalled bloatware on the OnePlus Nord Indian variant, that is either unusable outside of India, or undesirable.

The uninstall commands use ADB via USB debugging, and don't require root. See the following to get ADB set up on your platform: https://www.xda-developers.com/install-adb-windows-macos-linux/

After setting up and seeing your device when using the adb devices command, you can enter any of the uninstall commands to remove the related application.

## OnePlus
In order: Red Cable Club, Cricket Scores, OnePlus Community, Card Package (for loyalty cards in shelf)  
```
adb shell pm uninstall --user 0 com.oneplus.membership  
adb shell pm uninstall --user 0 com.oneplus.opsports  
adb shell pm uninstall --user 0 net.oneplus.forums  
adb shell pm uninstall --user 0 com.oneplus.card
```

## Google  
In order: Google Pay (Indian only variant), YouTube Music, YouTube
```
adb shell pm uninstall --user 0 com.google.android.apps.nbu.paisa.user
adb shell pm uninstall --user 0 com.google.android.apps.youtube.music
adb shell pm uninstall --user 0 com.google.android.youtube

```

## Facebook  
In order: Facebook, Facebook deleted data, Facebook System, Facebook Services, Updater for Facebook  
*Please note that com.facebook.system and com.facebook.appmanager may be required for the Oculus store.
```
adb shell pm uninstall --user 0 com.facebook.katana  
adb shell pm uninstall --user 0 com.facebook.orca  
adb shell pm uninstall --user 0 com.facebook.system  
adb shell pm uninstall --user 0 com.facebook.services  
adb shell pm uninstall --user 0 com.facebook.appmanager 
```
