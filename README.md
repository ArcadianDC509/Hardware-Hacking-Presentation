# Hardware Hacking 

This is a repo containing links and resources for good starting points to get into hardware hacking.


## Hardware Tools
- The CH341a programmer used for flashing and dumping firmware from EEPROM: https://www.amazon.com/HiLetgo-Programmer-CH341A-Burner-EEPROM/dp/B014VSGH4Y
- The DSD TECH SH-U09C2 USB debugger used to connect to SPI/UART interfaces: https://www.amazon.com/DSD-TECH-SH-U09C2-Debugging-Programming/dp/B07TXVRQ7V

## Software Tools


## Writeups and Blogs
Here is a great blog post from Black Hills Information Security on how to dump firmware from routers
https://www.blackhillsinfosec.com/dumping-firmware-with-the-ch341a-programmer/

## Notes and Caveates
- Devices that require more memory do not use EEPROM for the main file system. However embeded devices that are small are likely to still use EEPROM as the primary memory location
- There are ways to get access to the file system through hardware debugging ports that use UART or SPI.
- Over the air updates are used to update firmware over the air, as the name implies, and can reduce the need to physically open up devices.


## Notes on file systems
- For some reason binwalk was having issues extracting some older squashfs file systems, will need to look into finding workarounds. Other file systems include UBI blobs
