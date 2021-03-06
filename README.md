# bm34a configuration for rhythm games

## rules.mk
```Makefile
# Changed build options
BOOTMAGIC_ENABLE = full      # (default: lite) Virtual DIP switch configuration
COMMAND_ENABLE = no          # (default: yes) Commands for debug and configuration
NKRO_ENABLE = yes            # (default: no) USB Nkey Rollover
RGBLIGHT_ENABLE = yes        # (default: no) Enable keyboard RGB underglow
UNICODE_ENABLE = yes         # (default: no) Unicode

# Debouncing per key
# On any state change, response is immediate,
# followed by DEBOUNCE milliseconds of no further input for that key
DEBOUNCE_TYPE = sym_eager_pk
DEBOUNCE = 5
```

## config.h
```C++
#define QMK_KEYS_PER_SCAN 43
#define USB_POLLING_INTERVAL_MS 1
#define FORCE_NKRO

// Chord splitting fix
// https://github.com/qmk/qmk_firmware/pull/10955
#define DEFER_KEYBOARD_REPORT_ENABLE
```
## layers
### layer 0
![ScreenShot](/screenshots/0.png?raw=true "Layer 0")
### layer 1
![ScreenShot](/screenshots/1.png?raw=true "Layer 1")
### layer 2
![ScreenShot](/screenshots/2.png?raw=true "Layer 2")
### layer 3
![ScreenShot](/screenshots/3.png?raw=true "Layer 3")
### layer 4
![ScreenShot](/screenshots/4.png?raw=true "Layer 4")
