Extra Grapfics: [https://github.com/rakenrowl7/yubikayfive](https://github.com/rakenrowl7/yubikayfive)

# yubikayfive
made some uvk5 font face. compatible with https://github.com/amnemonic/Quansheng_UV-K5_Firmware/tree/main/font_and_graphics/encoder

[Download](https://github.com/rakenrowl7/yubikayfive)


**UV-K5 Stock **

Alphabet [(Modern DOS 8x16)](https://notabug.org/HarvettFox96/ttf-moderndos): ![760x16 stock](https://github.com/rakenrowl7/yubikayfive/blob/main/760x16%20stock.png)

BigDigits: ![bigdigits stock](https://github.com/rakenrowl7/yubikayfive/blob/main/bigdigits%20stock.png)

SmallDigits: ![84x8 stock](https://github.com/rakenrowl7/yubikayfive/blob/main/84x8%20stock.png)

**Atari ST 8x16**

Alphabet: ![760x16 atari](https://github.com/rakenrowl7/yubikayfive/blob/main/760x16%20atari.png)

BigDigits: ![bigdigits atari](https://github.com/rakenrowl7/yubikayfive/blob/main/bigdigits%20atari.png)

**Unifont Medium**

Alphabet: ![760x16 unifont](https://github.com/rakenrowl7/yubikayfive/blob/main/760x16%20unifont.png)

BigDigits: ![bigdigits unifont](https://github.com/rakenrowl7/yubikayfive/blob/main/bigdigits%20unifont.png)

**Microsoft Default Monospace Font**

Alphabet: ![760x16 mono](https://github.com/rakenrowl7/yubikayfive/blob/main/760x16%20mono.png)

BigDigits: ![bigdigits mono](https://github.com/rakenrowl7/yubikayfive/blob/main/BigDigits%20mono.png)

SmallDigits: ![84x8 mono](https://github.com/rakenrowl7/yubikayfive/blob/main/84x8%20mono.png)

**Microsoft Default Monospace Bold Font**

Alphabet: ![760x16 mono](https://github.com/rakenrowl7/yubikayfive/blob/main/760x16%20mono%20bold.png)

BigDigits: ![bigdigits mono](https://github.com/rakenrowl7/yubikayfive/blob/main/BigDigits%20mono%20bold.png)

SmallDigits: ![84x8 mono](https://github.com/rakenrowl7/yubikayfive/blob/main/84x8%20mono%20bold.png)

**[SperryPC](https://int10h.org/oldschool-pc-fonts/fontlist/?2#sperry)**

Alphabet: ![](https://github.com/rakenrowl7/yubikayfive/blob/main/760x16%20sperrypc.png)

SmallDigits: ![84x8](https://github.com/rakenrowl7/yubikayfive/blob/main/84x8%20sperrypc.png)
<hr>
Very first attempt to automate custom fonts generation. For now only for big digits in very crude and convoluted way.
Requirements: [Pillow](https://pypi.org/project/Pillow/) library.

<hr>

### BigDigits
<p align="center">
  <img  src="https://raw.githubusercontent.com/amnemonic/Quansheng_UV-K5_Firmware/main/font_and_graphics/encoder/BigDigits_VCR_font.png">
</p>

9 symbols, each of width=13px, height=16px, in firmware version `k5_2.01.26` at offset `0xD502`, 286 bytes in total.

Usage:

```
BigDigits_encode.py BigDigits_VCR_font.png mod_custom_bigdigits.py
```

as a result you should get file `mod_custom_bigdigits.py` which can be used in [uvmod_kitchen](https://github.com/amnemonic/Quansheng_UV-K5_Firmware/blob/main/uvmod_kitchen/)
<hr>

### Alphabet
<p align="center">
  <img  src="https://raw.githubusercontent.com/amnemonic/Quansheng_UV-K5_Firmware/main/font_and_graphics/encoder/Alphabet_Stock_Font.png">
</p>

95 symbols, each of width=8px, height=16px, in firmware version `k5_2.01.26` at offset `0xD66D`, 1520 bytes in total.

Usage:
```
Alphabet_encode.py Alphabet_Stock_Font.png mod_custom_alphabet.py
```

as a result you should get file `mod_custom_alphabet.py` which can be used in [uvmod_kitchen](https://github.com/amnemonic/Quansheng_UV-K5_Firmware/blob/main/uvmod_kitchen/)
<hr>

### symbols
<p align="center">
  <img  src="https://raw.githubusercontent.com/amnemonic/Quansheng_UV-K5_Firmware/main/font_and_graphics/encoder/Symbols_stock.png" width="884" height="16">
</p>

few symbols, various width, height=8px, in firmware version `k5_2.01.26` at offset `0xD348`, 442 bytes in total.

Usage:
```
Symbols_encode.py Symbols_stock.png mod_custom_symbols.py
```

as a result you should get file `mod_custom_symbols.py` which can be used in [uvmod_kitchen](https://github.com/amnemonic/Quansheng_UV-K5_Firmware/blob/main/uvmod_kitchen/)
<hr>
