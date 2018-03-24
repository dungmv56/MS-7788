# MS-7788

## Post installing
1. Copy kexts to /Library/Extensions
   sudo cp -r files/kexts/Library/Extensions/*.kext /Library/Extensions
   cd /Library/Extensions
   sudo chmod -R 755 *.kext
   sudo chown -R root:wheel *.kext
   sudo kextcache -i /
2. Install Clover bootloader (make sure install to ESP)
3. Using Clover Configurator to mount EFI partition
   Replace config.plist to /EFI/CLOVER/config.plist
   Delete some files in /EFI/CLOVER/drivers64 if necessary
4. Install VoodooHDA Classic
5. Have fun ;)
