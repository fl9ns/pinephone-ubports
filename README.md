### JUMPDRIVE on SD card

# get last img https://github.com/dreemurrs-embedded/Jumpdrive/releases
# decompress
xz -d pine64-pinephone.img.xz
# lsblk
sudo dd if=pine64-pinephone.img of=/dev/sdX bs=4M status=progress conv=fsync
