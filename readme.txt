avrdude -v -p atmega1284p -c arduino -P com6 -b 115200 -D -U flash:w:"anycubic_mega_zero_mbl-0.0.4-firmware.hex":i

avrdude -v -p atmega1284p -c arduino -P com6 -b 115200 –p m8 -D -U flash:w:"anycubic_mega_zero_mbl-0.0.4-firmware.hex":i

// read setings: avrdude -p atmega1284p -c arduino -P com6 -b115200 -Ueeprom:r:'printer_eeprom'.eep:i
