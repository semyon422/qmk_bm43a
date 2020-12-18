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
# On any state change, response is immediate, followed by DEBOUNCE milliseconds of no further input for that key
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
