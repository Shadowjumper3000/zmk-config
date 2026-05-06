# nice!view

The nice!view is a low-power, high refresh rate display meant to replace I2C OLEDs traditionally used.

This shield requires that an `&nice_view_spi` labeled SPI bus is provided with _at least_ MOSI, SCK, and CS pins defined.

## Disable custom widget

The nice!view shield includes a custom vertical widget. To use the built-in ZMK one, add the following item to your `.conf` file:

```
CONFIG_ZMK_DISPLAY_STATUS_SCREEN_BUILT_IN=y
CONFIG_ZMK_LV_FONT_DEFAULT_SMALL_MONTSERRAT_26=y
CONFIG_LV_FONT_DEFAULT_MONTSERRAT_26=y
```

## Rotate screen

You can rotate the custom widget by 180 degrees. To do so, add the following item to your `.conf` file:

```
CONFIG_NICE_VIEW_DISP_ROTATE_180=y

## Custom art

You can provide a custom image for the widget by adding a C header that defines an LVGL image descriptor named `nice_view_custom_art`.

1. Create a header (example: `nice_view_custom_art.h`) that contains an `lv_img_dsc_t` named `nice_view_custom_art` (many image-to-C tools can generate this for you).
2. Enable the custom art in your .conf:

```text
CONFIG_NICE_VIEW_DISP_CUSTOM_ART=y
```

3. If your header isn't in the include path or has a different name, set the path:

```text
CONFIG_NICE_VIEW_DISP_CUSTOM_ART_PATH="path/to/nice_view_custom_art.h"
```

When enabled, the widget will use `nice_view_custom_art` instead of the built-in balloon/mountain images.
```
