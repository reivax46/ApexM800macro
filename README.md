# ApexM800macro

### Support for Steelseries Apex M800 macro keys on linux. ###

Tested on Debian Jessie.

Originally circles keys on my Apex M800 keyboard were sending same keycodes as the multimedia keys. So I couldn't use them to achieve macros.
This file remaps circle keys 0 to 5 scancodes to unused keycodes.

### Installation ###

1. Move 90-apexm800.hwdb file to /etc/udev/hwdb.d directory
2. Run ``` sudo udevadm hwdb --update ```
3. Run ``` sudo udevadm control --reload ```
4. unplug and replug your keyboard

You can then create custom shortcuts for circle 0-5 keys in your desktop environment to achieve macros (for example with [xdotool](https://www.semicomplete.com/projects/xdotool/xdotool.xhtml)).
