# Installation for Raspberry Pi

[Guide](https://www.raspberrypi.com/documentation/computers/getting-started.html)

- Install Raspberry Pi Imager
- Install Raspberry OS into SD Card
- Access SD Card content
  - create file name: 
```
cd /Volumes/boot
touch ssh
```
- Insert Card into Raspberry Pi & power it on
- [Connect Raspberry Pi without Monitor](https://www.raspberrypi.com/documentation/computers/remote-access.html#nmap-command)
  - install nmap
  - scan all in Network: `nmap -sn 192.168.1.0/24`
- ssh into Raspberry: `ssh pi@<ip-from-nmap>` (password: raspberry)
- enable VNC Server in Raspberry
```
sudo raspi-config
-> Interface Options
-> VNC
-> Yes
```
- Use VNC to connect to Raspberry