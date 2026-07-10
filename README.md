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

```
### CHUM

# https://chumrpm.netlify.app/
# get sailfishos-chum-gui (aarch64)
# root
devel-su
# install with dependance
pkcon install-local sailfishos-chum-gui-0.6.12-1.13.1.bso.aarch64.rpm
reboot

vim ~/.local/share/applications/chum-custom.desktop
[Desktop Entry]
Type=Application
Name=Chum
Exec=sailfishos-chum-gui
Icon=icon-m-cloud-download
X-Hacks-ShowInLauncher=true
X-Nemo-Application-Type=silica-qt5

update-desktop-database ~/.local/share/applications

# install waydroid and waydroid runner
```
