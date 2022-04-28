# Air Quality Monitor
Measure air quality (PM2.5 and PM10) with a SDS011 particle sensor on a Raspberry Pi. Units reported in μg/m3.

Tested on Ubuntu Server 20.04.4 LTS, Python 3.8.10. PRs welcome.

## Installation

Check primary user for USB access:
```
groups USERNAME
```
If needed, add the following groups to grant USB access, then logout/login to update the group permissions:
```
sudo usermod -a -G tty USERNAME
sudo usermod -a -G dialout USERNAME
```
```
sudo restart
```

Install dependencies:
```
sudo apt install python3-pip
pip3 install pyserial
```

Install PM Monitor:
```
git clone https://github.com/dcato98/pi-pm-monitor
```
