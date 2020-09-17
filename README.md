# OnePlus Nord Debloat List

This is a list of preinstalled bloatware on the OnePlus Nord Indian variant, that is either unusable outside of India, or undesirable.

## OnePlus
In order: Red Cable Club, Cricket Scores, OnePlus Community, Card Package (for loyalty cards in shelf)  
>adb shell pm uninstall --user 0 com.oneplus.membership  
>adb shell pm uninstall --user 0 com.oneplus.opsports   
>adb shell pm uninstall --user 0 net.oneplus.forums  
>adb shell pm uninstall --user 0 com.oneplus.card