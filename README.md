# Corne Choc Pro ZMK Config

This repository contains the ZMK configuration for the Corne Choc Pro keyboard with a QWERTZ layout. The configuration includes multiple layers: Default, Number, and Symbol.

## Layers and Key Mappings

### Default Layer (QWERTZ)
```
--------------------------------------------------------------------------------
|  TAB |  Q  |  W  |  E  |  R  |  T  |       |       |  Z  |  U   |  I  |  O  |  P  | BSPC |
| CTRL |  A  |  S  |  D  |  F  |  G  |       |       |  H  |  J   |  K  |  L  |  -  |  '   |
| SHFT |  Y  |  X  |  C  |  V  |  B  |               |  N  |  M   |  ,  |  .  |  /  | ESC  |
                   | GUI | LWR | SPC |               | ENT | RSE  | ALT |
```

### Number Layer
```
-----------------------------------------------------------------------------------------
|     |     |STUNL| BOOT| RGB  | RST  |      |      |  7   |  8   |  9   |  =   |  %   |      |
|     | LEFT| DOWN|  UP | RIGHT|      |      |      |  4   |  5   |  6   |  /   |  *   |      |
|     |  F1 |  F2 |  F3 |  F4  |  F5  |             |  1   |  2   |  3   |  +   |  -   |      |
                  |     |      |      |             |  0   |      |      |
```

### Symbol Layer
```
-----------------------------------------------------------------------------------------
|BT_SEL 0|   ä  |  ß  |  ^  |  $  |  ?  |      |       |  '  |  [  |  ]  | volu| vold|   Delete    |
|BT_SEL 1|   ö  |  |  |  @  |  #  |  &  |      |       |  "  |  (  |  )  | c_pp|c_nxt|   Page Up   |
|BT_NEXT |   ü  |  ~  |  <  |  >  |  !  |              |  _  |  {  |  }  |     |     |   Page Down |
                      |     |     |     |              |     |     |     |
```

## How to Use

1. Clone this repository to your local machine.
2. Flash the firmware to your Corne Choc Pro keyboard using the ZMK build system.
3. Enjoy your custom QWERTZ layout!

## License

This configuration is licensed under the MIT License. See the `LICENSE` file for details.