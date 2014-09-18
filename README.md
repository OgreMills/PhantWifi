PhantWifi
=========

This sketch was created for uploading info to Sparkfun's data logging service (Phant) using an Arduino Wifi shield.
There is a tutorial on their page that shows how to do this for other shields like ethernet and so on, but not one 
based on this shield. I figured I'd upload it to help someone get a start with the service.


Use IDE 1.0.3 if you have a shield with chip HDG204.

The public and private key are used to post to the tutorial site on data.sparkfun.com
------- https://data.sparkfun.com/streams/6JZbNolApzF4om2l9yYK -------

You should replace the SSID and PW to fit your network settings.

Hardware Hookup:
  * These components are connected to the Arduino's I/O pins:
    * D3 - Active-low momentary button (pulled high internally)
    * A0 - Photoresistor (which is combined with a 10k resistor
           to form a voltage divider output to the Arduino).
    * D5 - SPDT switch to select either 5V or 0V to this pin.
  * A Arduino WiFi shield to put ontop of your Ardunio of choice.
  

Much of this code is largely based on David Mellis' WebClient example in the Ethernet library.
Also Jim Lindblom @ SparkFun Electronics
Original Creation Date: July 3, 2014
Modified: Sept 19th, 2014


Distributed as-is; no warranty is given.
