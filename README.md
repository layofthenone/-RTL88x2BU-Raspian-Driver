# [Asus USB ac58-1300]("https://www.asus.com/Networking-IoT-Servers/Adapters/All-series/USB-AC58/") Raspbian Driver
rtl88x2BU_WiFi_linux_v5.8.7.4 Raspberry Pi OS Driver Setup

# Update source list
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
git clone https://github.com/layofthenone/asus-ac58-raspbian-driver.git
```
```
cd asus-ac58-raspbian-driver/
```

### Unrar Rar File
```
unrar x rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777.rar
cd rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777/
```

### Install rtl88x2BU Driver
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
