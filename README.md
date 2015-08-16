Custom Marlin Firmware with Panelolu2 support for Dagoma #Discovery200 DIY printer with Melzi Ardentissimo
===================



License
===================

Marlin has a GPL license because we believe in open development.
Please do not use this code in products (3D printers, CNC etc) that are closed source or are crippled by a patent.


Quick Information
===================
This RepRap firmware is a mashup between <a href="https://github.com/kliment/Sprinter">Sprinter</a>, <a href="https://github.com/simen/grbl/tree">grbl</a> and many original parts.

Derived from Sprinter and Grbl by Erik van der Zalm.
Sprinters lead developers are Kliment and caru.
Grbls lead developer is Simen Svale Skogsrud. Sonney Jeon (Chamnit) improved some parts of grbl
A fork by bkubicek for the Ultimaker was merged, and further development was aided by him.
Some features have been added by:
Lampmaker, Bradley Feldman, and others...


Features:
=========

*   Interrupt based movement with real linear acceleration
*   High steprate
*   Look ahead (Keep the speed high when possible. High cornering speed)
*   Interrupt based temperature protection
*   preliminary support for Matthew Roberts advance algorithm
    For more info see: http://reprap.org/pipermail/reprap-dev/2011-May/003323.html
*   Full endstop support
*   SD Card support
*   SD Card folders (works in pronterface)
*   SD Card autostart support
*   LCD support (ideally 20x4)
*   LCD menu system for autonomous SD card printing, controlled by an click-encoder.
*   EEPROM storage of e.g. max-velocity, max-acceleration, and similar variables
*   many small but handy things originating from bkubicek's fork.
*   Arc support
*   Temperature oversampling
*   Dynamic Temperature setpointing aka "AutoTemp"
*   Support for QTMarlin, a very beta GUI for PID-tuning and velocity-acceleration testing. https://github.com/bkubicek/QTMarlin
*   Endstop trigger reporting to the host software.
*   Updated sdcardlib
*   Heater power reporting. Useful for PID monitoring.
*   PID tuning
*   CoreXY kinematics (www.corexy.com/theory.html)
*   Delta kinematics
*   SCARA kinematics
*   Dual X-carriage support for multiple extruder systems
*   Configurable serial port to support connection of wireless adaptors.
*   Automatic operation of extruder/cold-end cooling fans based on nozzle temperature
*   RC Servo Support, specify angle or duration for continuous rotation servos.
*   Bed Auto Leveling.

The default baudrate is 250000. This baudrate has less jitter and hence errors than the usual 115200 baud, but is less supported by drivers and host-environments.

Buying link
===================
**Dagoma** #discovery200 • Buy it [here](http://www.dagoma.fr/shop/)

**Panelolu2** • Buy it [here](http://www.think3dprint3d.com/Panelolu2)

Configuring and compilation:
============================

**01.** Turn off the printer and unplug the power cable.

**02.** Plug the usb cable between your computer and the #discovery200.

**03.** Install the **auto-reset jumper** on both pins.

**04.** Install the other jumper on **usb** (originally on  « VREG » – Voltage Regulation).

**05.** Download [Arduino 1.0.6](https://www.arduino.cc/en/Main/OldSoftwareReleases)

**06.** Copy the Arduino addons in your Arduino documents folder (hardware and library).

**07.** In Arduino 1.0.6 ("Tools" menu item) choose the board **Melzi W/ ATmega1284p 16mhz**.

**08.** In Arduino 1.0.6 ("Tools" menu item) choose the serial port **/dev/cu.usbserial-AH01SJ4P**.

**09.** Click the **Verify/Compile** button.

**10.** If succeed, click the **Upload** button.

**11.** If all goes well the firmware is uploading ;)

**12.** If uploading succeed **unplug usb cable.**

**13.** **Put the jumpers on their original position** (auto-reset OFF and mode VREG).

**14.** **Plug the power cable** on the #discovery200.
**15.** Happy printing with **#discovery200** and **Panelolu2!**

