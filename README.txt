A group project for a software design class, this app allows users to view the current time, weather, and their most recently played Spotify tracks and Twitter timeline. 

This version of this app requires an Arduino and Raspberry Pi to display the UI via an LCD screen as the intended final design for this project.

LIBRARY INSTALLATION:
sudo apt-get update -y
sudo apt-get install libcurl4-openssl-dev
sudo apt-get install wiringpi
sudo apt-get install build-essential
sudo apt-get install qt5-default
sudo apt-get install libjsoncpp-dev

WIRING:
----ARDUINO----
LED VCC to ARDUINO DIG PIN 13
LED GND to ARDUINO GND
PIR OUTPUT to ARDUINO DIG PIN 3
PIR VCC to ARDUINO 5V
PIR GND to ARDUINO GND

----RASPBERRY PI----
Arduino USB B to Raspberry Pi USB A
Display HDMI to Raspberry Pi HDMI

COMPILE & RUN:
find . -exec touch {} \;
qmake
make
./SmartMirror
