Firmware version spoofing modded firmware v2 for v3, v4 uv-5r plus

1. Download file qsfirm.py
place it into the same folder with k5_v2.01.26_mod.bin

2. Run command: qsfirm.py unpack k5_v2.01.26_mod.bin fw.dec.bin fw.ver.bin

3. Edit file fw.ver.bin in hex editor to start with 4, for example 4.00.1

4. Run command: qsfirm.py pack fw.dec.bin fw.ver.bin k5_v2.01.26_mod_v4.bin
