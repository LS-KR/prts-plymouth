# prts-plymouth

Rhodes Island PRTS loading slash animation

![Generated Gif](doc/120015.gif)

## Installation

``` bash
# Clone this repo
git clone https://github.com/LS-KR/prts-plymouth.git
cd prts-plymouth

# Install theme
sudo mkdir /usr/share/plymouth/themes/prts
sudo cp -rf animated-boot.script prts.plymouth img /usr/share/plymouth/themes/prts/

# Enable this theme
sudo plymouth-set-default-theme prts

# For show once: run this as root
plymouthd;plymouth show-splash futureprototype;sleep 5;plymouth --quit
```

then regenerate your initramfs.