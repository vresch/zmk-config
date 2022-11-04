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
6. Reset the keyboard (Single-click RESET btn on both splits)
7. Connect the keyboard via Bluetooth. Test. Enjoy!

## Reference
- [1] Installing ZMK
https://zmk.dev/docs/user-setup
- [2] Layer model description
https://zmk.dev/docs/behaviors/layers
- [3] Troubleshooting
https://zmk.dev/docs/troubleshooting
## Topics
split-keyboard orthogonal-keyboard flashing-utility