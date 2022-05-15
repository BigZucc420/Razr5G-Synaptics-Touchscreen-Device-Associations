# Razr5G Synaptics Touchscreen Device Associations (magisk)
A magisk module that helps the cli display's touchscreen work correctly on GSIs.

This module has been tested on my XT2071-3 but is not guaranteed to work on your XT2071-3.

What the module does:
- maps the internal touch screen to the internal display port and the cli touch screen to the cli display port in `input-port-associations.xml`

Bugs:
- for whatever reason, `a2dp_audio_policy_configuration.xml` and `audio_policy_configuration.xml` can get overwritten, breaking audio (I'm working on a fix for that)
- more that I'm probably missing...

Other things:
- this might not work on your device if your device's touch screen hardware or display identifiers are different
- you will need to install this magisk module to display the system on the cli display: https://github.com/BigZucc41/Razr5G-Foldable-Device-Fixes
- this is not a part of the Foldable Device Fixes module because I'm going to be releasing other ways of getting a UI on the second display that are similar to the stock firmware

Sources:
- AOSP official documentation (https://source.android.com/devices/tech/display/multi_display/input-routing)
- Magisk documentation (https://github.com/BigZucc41/Razr5G-Foldable-Device-Fixes)
