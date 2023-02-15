# PWO Secure Industrial Network

In this research project we focus on informing the workfield aboud vulnerabilities in there OT-IT systems.

To demonstrate this we build a demo-setup.

![images](./images/image1.png)

## Setting up the Raspberry Pi

### OS Raspberry Pi

- Install `Raspberry Pi OS` on the SD card with Raspberry Pi Imager.
- Boot the Raspberry Pi and select your user/password. For this project we used `pi` & `pwosin`.
- Setup the static IP adres
```bash
sudo nano /etc/dhcpcd.conf
```
Change the following:
```conf
interface eth0
static ip_address=172.16.12.42/16
static routers=172.16.0.0/16
static domain_name_servers=193.190.147.185
```
Use Ctrl-X to save and exit.

- Then reboot the Pi:
```bash
sudo reboot -h 0
```
