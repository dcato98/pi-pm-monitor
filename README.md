# Air Quality Monitor
Measure AQI based on PM2.5 or PM10 with a Raspberry Pi and a SDS011 particle sensor. 

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
