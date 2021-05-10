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


