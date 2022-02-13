# [ASUS AC1300 USB-AC55 B1]**asd**
ASUS U2
ASUS USB-AC53 Nano
ASUS USB-AC58 Raspbian Driver
rtl88x2BU_WiFi_linux_v5.8.7.4 Raspberry Pi OS Driver Setup

## Setup Raspbian 
#### with this tutorial [link](https://www.tomshardware.com/reviews/raspberry-pi-set-up-how-to,6029.html)

## Update source list
```
sudo nano /etc/apt/sources.list
```
```
# Uncomment line below then 'apt-get update' to enable 'apt-get source'
deb http://raspbian.raspberrypi.org/raspbian/ buster main contrib non-free rpi
#deb-src http://raspbian.raspberrypi.org/raspbian/ buster main contrib non-free rpi
#deb http://archive.raspbian.org/raspbian wheezy main contrib non-free
#deb-src http://archive.raspbian.org/raspbian wheezy main contrib non-free
#deb http://mirrordirector.raspbian.org/raspbian/ jessie main contrib non-free rpi
#deb http://mirrordirector.raspbian.org/raspbian wheezy main contrib non-free firmware rpi
deb http://archive.raspberrypi.org/debian/ buster main
#deb-src http://raspbian.raspberrypi.org/raspbian/ buster main contrib non-free rpi
```

### Update Raspbian
```
sudo apt update
sudo apt upgrade
```

### Reboot OS
```
sudo reboot
```
### Setup Unrar
```
sudo apt-get install unrar-free unrar
```

### Download Driver
```
git clone https://github.com/layofthenone/RTL88x2BU-Raspian-Driver.git
```
```
cd asus-ac58-raspbian-driver/
```

### Unrar Rar File
```
unrar x rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777.rar
cd rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777/
```

## Install rtl88x2BU Driver
```
sudo make
```
```
sudo make install
```
```
sudo reboot
```
### and DONE




# Share Your Network
### If you want to setup your wifi hotspot(wifi-to-wifi) or wifi to eth bridge
`
https://github.com/arpitjindal97/raspbian-recipes
`
