# USB-HID-VolumeControl-RPi-PICO
USB HID Volume Control with Rotary Encoder Input using PICO-SDK

Platform : Raspberry Pi PICO

This is a modified version of the Keyboard and Mouse example of tinyUSB library named "hid_multiple_interface".
The rotary encoder can be used to increase/decrease the volume or mute it.
The pico board can be plugged in to Windows, Linux machine or even Android smartphone.

To build copy the file "main.c" to the path :
(After saving the original file as "main.c.orig")
	
	/pico-sdk/lib/tinyusb/examples/device/hid_multiple_interface/src

and build by running :

	cd /pico-examples/build/ 
	cmake .. 
	cd /pico-examples/build/usb/device/tinyusb_device_examples/hid_multiple_interface
	make


Rotary Encoder#	GPIO#	Board Pin

CLK (A)#	GP20# 	26

DT (B)#		GP21#	27

SW#		GP22#	29

VCC#			36

GND#			38


Rotate Clockwise=		Volume UP

Rotate Counterclockwise=	Volume DOWN

Press=				MUTE


Please let me know if you face any issues.
