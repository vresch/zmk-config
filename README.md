# ZMK firmware config for bluetooth chip nice!nano v2.0:
- kyria.keymap

## Description
It's a custom config for Kyria split ortho keyboard.
Adapted for Cyrilic Languages keymap.
- L0 Letter layer
- L1 Numbers and special characters layer
- L2 Navigation layer

Layers switched by tap.

## Flashing flow
1. Install ZMK [1]
```
bash -c "$(curl -fsSL https://zmk.dev/setup.sh)"
```

2. Modify & save "kyria.keymap"
3. Push to remote repo
```
git add .
git commit
git push
```
4. Download flashed .uf2 file after successful built on GitHub Actions (eg. https://github.com/vresch/zmk-config/actions)
5. Connect kbrd parts via USB one-by-one (Double-click RESET btn on a split to activate flash mode) and transfer firmware files accordingly
```
cp ~/dev/zmk-config/firmware/kyria_right-nice_nano_v2-zmk.uf2 /Volumes/NICENANO/
```
6. Reset the keyboard (Single-click RESET btn on both splits)
7. Connect the keyboard via Bluetooth. Test. Enjoy!

## Reference
- [1] Installing ZMK
https://zmk.dev/docs/user-setup
- [2] Layer model description
https://zmk.dev/docs/behaviors/layers
- [3] Troubleshooting
https://zmk.dev/docs/troubleshooting
- [4] Troubleshooting: macos bluetooth keyboard passkey missmatch
https://discussions.apple.com/thread/253818795
Connect the USB keyboard and mouse to the computer.
Open System Preferences – Bluetooth
Un-pair the wireless keyboard and mouse.
Turn off Bluetooth
Restart the computer in Safe Mode per the directions in How to use safe mode on your Mac - Apple Support
Restart the computer normally.
Open System Preferences – Bluetooth
Turn on Bluetooth
Re-Pair the wireless keyboard and mouse.
Unplug the USB keyboard and mouse and begin testing the wireless devices again. 
## Topics
split-keyboard orthogonal-keyboard flashing-utility