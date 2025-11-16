**pi-fm-rds-web**

A Web-Controlled FM Transmitter Toolkit for Raspberry Pi

pi-fm-rds-web is a web-configurable FM radio transmitter system for Raspberry Pi.

It automatically installs PiFmRds, sets up systemd services, and provides a clean, mobile-friendly dashboard on port 8080 to manage everything.

Basically it makes your pirate radio a breeze to setup

-----------------------------------------
**Features**:

- FM Frequency
- RDS Station Name (PS)
- RDS Radio Text (RT)
- Audio source filepath (.wav)
- Automatic looping playback
- Full auto-start at boot


<img width="670" height="456" alt="image" src="https://github.com/user-attachments/assets/1c18de26-1d9b-4a69-9eb7-2a4d3428f769" />

-----------------------------------------

**Installation**

wget https://github.com/SixtyAteWhiskey/pi-fm-rds-web/blob/main/pi-fm-rds-web.deb

sudo apt install ./pi-fm-rds-web.deb

-----------------------------------------

**Hardware Requirements**

Raspberry Pi (Zero W, 2, 3, 4, or 5)

20–30 cm wire connected to GPIO 4 (Pin 7)

Breadboard jumper wire works great for this!

I'll be creating a video for this at which point I'll link it here!

**Commands**

Restart the service

sudo systemctl restart pirateradio.service


Restart web app

sudo systemctl restart pirateradio-web.service


Check status

systemctl status pirateradio.service


Edit config manually

sudo nano /opt/pirateradio/radio.conf
