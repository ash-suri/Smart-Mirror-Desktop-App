This version of this app requires an Arduino and Raspberry Pi to display the UI via an LCD screen.

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
