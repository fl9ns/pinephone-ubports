```
### TWO BOOT

# get last img https://github.com/Tow-Boot/Tow-Boot/releases
# decompress
# lsblk
sudo dd if=mmcboot.installer.imgof=/dev/sdX bs=4M status=progress conv=fsync
```



```
### JUMPDRIVE on SD card

# get last img https://github.com/dreemurrs-embedded/Jumpdrive/releases
# decompress
xz -d pine64-pinephone.img.xz
# lsblk
sudo dd if=pine64-pinephone.img of=/dev/sdX bs=4M status=progress conv=fsync
```


```
### FLASH IT SailfishOS

# get script https://github.com/sailfish-on-dontbeevil/flash-it
# run script and choice Pinephone 1.2 (#2)
```
