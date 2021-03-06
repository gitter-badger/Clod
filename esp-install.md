ESP8266 Installation
====================

Wiring and Flashing
-------------------

This guide assumes you have some knowledge of how to flash microprocessors using FTDI serial communication. This includes basic knowledge of electrical circuits, resistors, and voltage regulators.

Follow [this excellent MAKE guide](http://makezine.com/2015/04/01/installing-building-arduino-sketch-5-microcontroller/) for the wiring section only, then come back here for the easiest way to flash it using Platform IO.


Using Platform IO
-----------------

* [Install Platform IO](http://docs.platformio.org/en/stable/installation.html)

* Download the Clod-sketch-library to your computer

* Open the Initial_Config folder within the Clod-sketch-library

	* File > Add Project Folder > Initial_Config

* Edit the definition file

	* On the left pane, expand `src` and open `ESPBoardDefs.h`

	* Change `String board_type = "esp01_1m";` to match the type of ESP board type you have. [List of available board types](http://docs.platformio.org/en/stable/platforms/espressif8266.html#espressif)

* Edit platformio.ini

	* Open the platformio.ini file

	* Make sure `board = esp01_1m` matches the definition file

* Click upload button (the rightward arrow on the top panel)

* Close the serial terminal, or remove the usb cable from your computer

* Power on the chip

* Follow the [rest](https://github.com/jakeloggins/Clod#getting-started) of this guide 

* Note: After completing this section, you will never need to connect the chip to your computer again (assuming nothing goes wrong).