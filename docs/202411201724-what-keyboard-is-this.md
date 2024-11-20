---
date: 2024-11-20 17:24
name: what keyboard is this
---

_***what keyboard is this***_

<https://usevia.com> reports `foostan Corne`

<https://github.com/foostan/crkbd> and in #257 (a pr to add to QMK) this is mentioned <https://github.com/foostan/kbd_firmware>

ah man its another repo? looks like theres a dependency on having qmk setup anyway

---

the desktop version of via mentions `CRKBD` which i think foostan/crkbd mentioned was short for "corne keyboard"

and now the list on <https://browse.qmk.fm/#/> has `crkbd/rev1` and `crkbd/r2g`

god knows which one i want - but im gonna hazard a guess and say rev1?

```fish
→ qmk compile -kb crkbd -km default
Ψ Compiling keymap with make -r -R -f builddefs/build_keyboard.mk -s KEYBOARD=crkbd/rev1 KEYMAP=default KEYBOARD_FILESAFE=crkbd_rev1 TARGET=crkbd_rev1_default VERBOSE=false COLOR=true SILENT=false QMK_BIN="qmk"

# ...


Linking: .build/crkbd_rev1_default.elf                                                              [OK]
Creating load file for flashing: .build/crkbd_rev1_default.hex                                      [OK]
Copying crkbd_rev1_default.hex to qmk_firmware folder                                               [OK]
Checking file size of crkbd_rev1_default.hex                                                        [OK]
 * The firmware size is fine - 25748/28672 (89%, 2924 bytes free) # 28.672 KB, 32KB avail. -> 89.6%
```

yikes! the default uses about 90% of the flash!
