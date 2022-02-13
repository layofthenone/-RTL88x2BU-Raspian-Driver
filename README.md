# asus-ac58-raspbian-driver
rtl88x2BU_WiFi_linux_v5.8.7.4 Raspberry Pi OS Driver Setup

sudo nano /etc/apt/sources.list

# Uncomment line below then 'apt-get update' to enable 'apt-get source'
deb http://raspbian.raspberrypi.org/raspbian/ buster main contrib non-free rpi
#deb-src http://raspbian.raspberrypi.org/raspbian/ buster main contrib non-free rpi
#deb http://archive.raspbian.org/raspbian wheezy main contrib non-free
#deb-src http://archive.raspbian.org/raspbian wheezy main contrib non-free
#deb http://mirrordirector.raspbian.org/raspbian/ jessie main contrib non-free rpi
#deb http://mirrordirector.raspbian.org/raspbian wheezy main contrib non-free firmware rpi
deb http://archive.raspberrypi.org/debian/ buster main
#deb-src http://raspbian.raspberrypi.org/raspbian/ buster main contrib non-free rpi

update raspbian
`
sudo rpi-update
sudo apt update
sudo apt upgrade
`

reboot os
`
sudo reboot
`
setup unrar
`
sudo apt-get install unrar-free unrar
`

download driver
`
git clone https://github.com/layofthenone/asus-ac58-raspbian-driver.git
`
`
cd asus-ac58-raspbian-driver/
`

unrar rar file
`
unrar x rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777.rar
cd rtl88x2BU_WiFi_linux_v5.8.7.4_37264.20200922_COEX20191120-7777/
`

`
sudo make
`
`
sudo install
`
`
sudo reboot
`

and done
