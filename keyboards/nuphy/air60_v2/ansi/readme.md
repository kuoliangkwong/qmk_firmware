c# NuPhy Air60 V2

*NuPhy Air60 V2 is a standard 64 key keyboard.*
![NuPhy Air60 V2](https://bit.ly/48qfjbS)

* Keyboard Maintainer: [nuphy](https://github.com/nuphy-src)
* Hardware Supported: NuPhy Air60 V2 PCB
* Hardware Availability: Private

Make example for this keyboard (after setting up your build environment):

    make nuphy/air60_v2/ansi:via

Flashing example for this keyboard:

    make nuphy/air60_v2/ansi:via:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in one way:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard


## Side Light Custom Color via VIA Support (Only works for Air60v2)
Follow these steps to change side light color:
1. Connect keyboard via USB.
2. Open [VIA](https://usevia.app/) and connect your keyboard.
3. Press ```FN + M + >``` to change the color mode from rainbow to custom color mode.
4. Change the light color in VIA. This will change your backlight. It is expected.
5. Press ```FN + M + Right CMD``` to sync the current backlight color from VIA to side light. (You could also assign a specific a key for this action. Look for ```Side Sync``` under ```Custom``` in ```Keymap```. Be sure to use the updated JSON file to update in ```Design``` tab in VIA, similar to this step 2 in [here](https://nuphy.com/pages/via-usage-guide-for-nuphy-keyboards)).
6. Now you are freely to adjust the color for key lights. To change side light color again, repeat steps 4-6.

**Limitations**
1. The color between backlight and sidelight might be different even they are set with the same color. Suspected Nuphy uses different LED for side light and backlight and makes them have different color result.
2. The side light color presets no longer available. This is more an enhancement to make the process simpler without cramping too many color presets.
3. Changing color in VIA does not reflect the color to side light immediately. The side light color will get updated after pressing ```FN + M + Right CMD``` (aka Side Sync key).

**Disclaimers**

Custom side light color is an unofficial feature made by me. There might be risk of bricking your keyboard using this firmware. Use it at your own risk as this is not tested thoroughly.
