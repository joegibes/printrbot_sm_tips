# printrbot_sm_tips
Printrbot Simple Metal rev F4 - running Klipper with extended heated X-axis and Ubis 13S. Tips, tricks, configs for PBSM and other Printrbots.


Included so far:
1. printer.cfg for my printer, with some comments explaining my changes.
2. Cura Profile "versatile jg1" - nice fast accel values for printing PLA with my Printrbot Simple Metal
3. Cura Pre/Post Gcode - basic setup and nozzle purge. Loads my bed_mesh_calibrate file (called 'default').

TODO:
1. Broken Fan Mosfet solution
    * Fan mosfet is small SMD, so I made a fan control circuit with a transistor/mosfet and use a different unused pin to control fan now.
    * Klipper is great for fan control since you can define custom fans, use any pin, even GPIO pins on the Raspberry Pi or other controller. (requires [setting up Pi as an additional MCU](https://www.klipper3d.org/RPi_microcontroller.html))


Helpful Links:

* https://www.brookdrumm.com/designs - 3D models for Printrbot and official upgrades/ accessories
    * [Printrbot Simple Metal A360 3D Model](https://a360.co/2UhjiS1) - you can export this in your format of choice, great for designing accessories/brackets/etc
* https://github.com/Printrbot - Printrbot official Github. Firmware info+.hex files, configs, printrboard eaglecad, various utilities
* http://www.reddit.com/r/Printrbot - subreddit
* The [Klipper Installation Page](https://www.klipper3d.org/Installation.html) ([or the Install page on github](https://github.com/KevinOConnor/klipper/blob/master/docs/Installation.md)) is excellent. If you've setup a raspberry pi before and/or flashed firmware onto a 3d printer, it's straightforward. 
* https://reprap.org/wiki/Printrboard - nice reference for the board schematic and pin listings. You can probably save your Configuration.h file from Marlin and use that to reference the pin assignments. This page doesn't list the Rev F6 though.

* [Nero 3dp - Klipper Initial Setup : Making sure things are all good before printing](https://www.youtube.com/watch?v=T-knWbh1Gg8) - this channel is excellent for Klipper stuff. I used his Input Shaper tuning guide with an accelerometer.

* [Generic Printrboard Klipper Config](https://github.com/KevinOConnor/klipper/blob/master/config/generic-printrboard.cfg) - I started with this but had to modify lots of stuff to get going. Mainly the pins to start.

* https://www.reddit.com/r/klippers/comments/ae74z6/need_help_installing_klipper/ - helpful thread
