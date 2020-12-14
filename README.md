
Assembly and setup of Raspberry Pi 4B
  
  Power supply:  At least 3.0 amps for Raspberry Pi 4
  
  A microSD card: Your Raspberry Pi needs an SD card to store all its files and the Raspbian operating system.
  
  You need a microSD card with a capacity of at least 8 GB.
  
  A keyboard and a mouse
  
  To start using your Raspberry Pi, you need a USB keyboard and a USB mouse.
  
  Once you’ve set your Pi up, you can use a Bluetooth keyboard and mouse, but you’ll need a USB keyboard and mouse for the first setup."
  
  A TV or computer screen
  
  To view the Raspbian desktop environment, you need a screen, and a cable to link the screen and the Pi. The screen can be a TV or a computer monitor. If the screen has built-   in speakers, the Pi is able to use these to play sound."
  
  HDMI
  
  The Raspberry Pi has a HDMI output port that is compatible with the HDMI port of most modern TVs and computer monitors. Many computer monitors may also have DVI or VGA ports.
  
  Raspberry Pi 4 has two micro HDMI ports, allowing you to connect two separate monitors. "
  
  Set up MicroSD Card
  https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up/2
  
  Connect Your Pi
  https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up/3
  
  Start It Up
  https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up/4
  
  Finish Setup
  https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up/5

  Obtain and install OS based on tutorials
Use this tutuorial or the book that came with the kit for camera installation
https://www.youtube.com/watch?v=qk1IVs5B1GI




Need to install camera and follow video

https://www.youtube.com/watch?v=qk1IVs5B1GI

For Raspbian

Install camera cable

Test Camera using Raspbian through Terminal

#raspistill -rot 180 -o test.jpg# BEcause camera cannot be mounted right side up at the moment 

Install and run picamera from Thonny IDE within Raspbian OS

#from picamera import PiCamera#

#from time import sleep#

#camera = PiCamera()#

#camera.rotation = 180#

then


#camera.start_preview()#

#sleep(5)#

#camera.capture('/home/pi/Desktop/image.jpg')

#camera.stop_preview()#

Click Run

This will allows to view and capture still images to your rasp pi

If program does not run correctly and capture image

Hold down ctrl+alt+t which will open up a terminal that has focus, although hidden behind the preview.

Then blindly type

pkill python3

Enter

For video use:


#from picamera import PiCamera#

#from time import sleep#

#camera = PiCamera()#

#camera.rotation = 180#

then


#camera.start_preview()#

#camera.start_recording('/home/pi/Desktop/video.h264')#

#sleep(10)#

#camera.stop_recording()#

#camera.stop_preview()#



Follow Tutorial for Connecting to Wifi

Wifi Config file is included in this repo (wpa-supplicant.conf)

Refer to this site for instructions and image for OS https://dronebotworkshop.com/motioneyeos-raspberry-pi/

https://github.com/ccrisan/motioneyeos/wiki/Supported-Devices for Supported Devices

Camera will streams through local internet to a local IP.  

ItShowTime Wiki contains link for supported device images

ksu-is/motioneyeos or to bdobson5/ItsShowTime.  The Wiki from source contains the various updates for newer gens of rasp pi. https://github.com/ccrisan/motioneyeos/wiki/Supported-Devices

https://github.com/ccrisan/motioneyeos/wiki

Build openCV as a precursor for a more advanced OS prodivded by

https://github.com/ksu-is/ItsShowTime/blob/main/SecCamREADME.md

https://github.com/ksu-is/opencv

Configure according to your needs with incredibly user friendly web browser GUI for MotionEyeOS





