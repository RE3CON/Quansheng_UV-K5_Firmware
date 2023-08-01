Firmware version spoofing

1. download file qsfirm.py
place it into the same folder with k5_v2.01.26_mod.bin

2. run command: qsfirm.py unpack k5_v2.01.26_mod.bin fw.dec.bin fw.ver.bin

3. edit file fw.ver.bin in hex editor to start with 4, for example 4.00.1

4. run command: qsfirm.py pack fw.dec.bin fw.ver.bin k5_v2.01.26_mod_v4.bin
