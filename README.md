# Dash Button Detection

This project uses an ESP8266 board to recognize the press of a dash button. 
It is based on the code from the [ESP8266 Wifi Sniffer project](https://github.com/kalanda/esp8266-sniffer).
The board is an [IoT Octopus](http://fab-lab.eu/octopus/).

**NOTE:** *This code is only for educational purposes.*

## Demo

![Demo Video](https://youtu.be/6cVYy-x6IMI)

## How it works

The button isn't modified. It is configured to connect to a Wifi network with the Amazon app. This wifi network was only set up temporarly, so that the button can not connect Amazon when it is pressed. However it will try to connect to the configured Wifi network. The Wifi sniffer code will recognize this attempt. The MAC address of the connecting device is checked. If it matches the MAC of the dash button the color of a NeoPixel LED is changed.

