# Supported Devices
rtl88x2BU_WiFi_linux_v5.8.7.4 Raspberry Pi OS Driver Setup
###### [ASUS USB-AC58 1300](https://www.asus.com/Networking-IoT-Servers/Adapters/All-series/USB-AC58/)
###### [ASUS USB-AC55_B1 1300](https://www.asus.com/Networking-IoT-Servers/Adapters/All-series/USB-AC55-B1/)
###### [ASUS USB-AC53 Nano 1200](https://www.asus.com/us/Networking-IoT-Servers/Adapters/All-series/USB-AC53-Nano/)

`I haven't tried with more devices, you can try devices on the same chipset`

# Setup Raspbian 
#### with this tutorial [link](https://www.tomshardware.com/reviews/raspberry-pi-set-up-how-to,6029.html)

# Setup RTL88xBU Raspbian Driver
## Update source list
```
sudo nano /etc/apt/sources.list
```
```
# Uncomment line below then 'apt-get update' to enable 'apt-get source'
deb http://raspbian.raspberrypi.org/raspbian/ buster main contrib non-free rpi
deb http://archive.raspberrypi.org/debian/ buster main
```

## Update Raspbian
```
sudo apt update
sudo apt upgrade
```

## Reboot OS
```
sudo reboot
```
## Setup Unzip
```
 sudo apt install unzip
```

## Download Driver
```
git clone https://github.com/layofthenone/RTL88x2BU-Raspbian-Driver.git
```
```
cd RTL88x2BU-Raspbian-Driver
```

## Extract From Rar File
```
unzip rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777.zip
cd rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777/
```

## Install Driver
```
sudo make
```
```
sudo make install
```
```
sudo reboot
```
### and Done




# Share Your Network
### If you want to setup your wifi hotspot(wifi-to-wifi) or wifi to eth bridge
with this [link](https://github.com/arpitjindal97/raspbian-recipes)
