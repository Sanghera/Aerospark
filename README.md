Rockoon Project
====================

This project was developed as an open source experiment of the “rockoon” concept.  The basic idea is to launch a rocket from a high altitude balloon at, or near, it’s burst altitude.  The purpose of this experiment is to demonstrate alternative technology to reach space.

A full overview of the technology and a detailed study of the concept is available in the PDF document titled “Design and Analysis of a Lunar Mission Launched From a High Altitude Balloon”.

The payload contains a Raspberry Pi with the Aerospark shield, and a RockBLOCK unit which plugs directly into the Pi’s USB port.  Once powered, load the code to the Pi, edit the desired altitude, and make sure you have credits on your RockBLOCK.  Once the altitude is reached, the ignition relay will close the ignition circuit and fire the rocket.  Tracking is provided by the Iridium satellite network which is published by RockBLOCK through HTTP requests to the Aerospark website.

If you have any questions, feel free to contact me at el.sanghera@gmail.com

Iridium SBD
================

This folder contains a few python and node.js scripts for communicating with a RockBLOCK Iridum unit.

In the python folder you will find a code to allow you to send simple commands to the RockBLOCK directly from the terminal window by running:
```
// python hello_iridium.py -d /dev/ttyUSB0
```
For a detailed list of all of the commands visit: http://tabs2.gerg.tamu.edu/~norman/659/9602DevelopersGuide_RevisionBEAM.pdf

To initiate a SBD session and transmit "Hello World" to the iridium network:
```
// python run_iridium.py -d /dev/ttyUSB0
```

The node.js folder was obtained from the RockBLOCK website, and can also be used for communicated with the RockBLOCK.


Flight Computer
============

The master flight computer code for the HAB/Rockoon launch is available in this code.

PCB
===

The Aerospark Printed Circuit Board is also available.  Eagle files are included in this folder.

Licence
======

[BSD Licence](http://opensource.org/licenses/bsd-license.php)
