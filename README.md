# Mega-zero-stock-frimware
This repository contains HEX file of stock frimware for anycubic MEGA ZERO 3D-printer

To instal stock frimware follow next steps:

1) Download repository 

2) downloar arduino ide? last version

3) add next link to manager boards:https://raw.githubusercontent.com/Lauszus/Sanguino/master/package_lauszus_sanguino_index.json

4)install sanguino from the boards manager, close arduino

5)create new floder, and copy there next files from arduino IDE floder: libusb0.dll, avrdude.conf, avrdude.exe, or use files from reposytore

6) add frimeware file from repository to this floder

7) write CMD in the adressbar of the floder

8) write in CMD next text to boot frimware:

avrdude -v -p atmega1284p -c arduino -P com6 -b 115200 -D -U flash:w:"anycubic_mega_zero_mbl-0.0.4-firmware.hex":i

or

avrdude -v -p atmega1284p -c arduino -P com6 -b 115200 –p m8 -D -U flash:w:"anycubic_mega_zero_mbl-0.0.4-firmware.hex":i

9) write in CMD next text to read eprom:

avrdude -p atmega1284p -c arduino -P com6 -b115200 -Ueeprom:r:'printer_eeprom'.eep:i

Support autor: qiwi.com/p/380937122470


