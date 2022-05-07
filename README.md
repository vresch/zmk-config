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

2. Make changes
3. Push to remote repo
4. Download flash u2 file after automatically built on GitHub Action
5. Reset the keyboard (splits)

## Reference
- [1] Installing ZMK
https://zmk.dev/docs/user-setup
- [2] Layer model description
https://zmk.dev/docs/behaviors/layers
- [3] Troubleshooting
https://zmk.dev/docs/troubleshooting
## Topics
split-keyboard orthogonal-keyboard flashing-utility