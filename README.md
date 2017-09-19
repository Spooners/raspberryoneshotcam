# raspberryoneshotcam
This project is a python script running on a Raspberry Pi 3.
It requires a servo motor and the picamera

Functional description:
The script is intended to run at boot time. First it will check if the Pi is connected to a WiFi network with a given SSID. 
If not, it will turn the servo in order to push the on/off button on a network modem to switch it on. Then wait and check for the WiFi network again.
If the network is available it will take one picture with the picam and upload it to a ftp server
Then it will turn the servo in order to push the on/off button on a network modem to switch it off.
Finally it will shut down the Pi
