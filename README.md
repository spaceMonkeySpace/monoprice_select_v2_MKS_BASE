# Upgrade  monoprice select v2 3D printer with a MKS SBASE board

## the monoprice select v2
The monoprice select v2 is an affordable 3 printer, but it comes with some flows. At the begginning it was printing right thrue SD card and USB and gradualy while the software (cura or repetier) goes on update, this closed source printer stopped to print. In adition some part went broken.
I purchase it knowing that issues will happen, and I planned to fix it with an open source 32bit board, and new quality part when one fail. 
And here we are

# new electronic breadboard
The MKS SBASE v1 is an affordable 32 bit board with good capabilities. It run the smoothieware firmare (this is open source and can be found here https://github.com/Smoothieware/Smoothieware). This is not marlin or repetier
Before unboxing the board this is very important to read the WHOLE documentation here https://smoothieware.org/3d-printer-guide
Because there is many way to fry the board, if like me you ruch the wiring. For exemple you must never unplug the stepper while the board is on.
The endstop connectors are not the same from the printer and on the board, a bad connection end up with the board destruction also (got me)

This repository is mainly used to keep an up to date configuration file dedicated to this printer. His is a work in progress , dont use as it until this desclaimer change. This is not a full instruction of how to do it :) but feel free to ask improvement I will help and document here.

# Resources
 * I am not the firt who done it, there a pretty well documented project here :  https://www.instructables.com/Monoprice-Select-Mini-Smoothieboard-Conversion/
 * complete guide for smoothieboard setup https://smoothieware.org/3d-printer-guide 
# TODO list :
- [x] tune current of the stepper https://mpselectmini.com/parts/stepper_motors
- [ ] fine tune current of the stepper https://mpselectmini.com/parts/stepper_motors
- [ ] fine tune step per mm
- [ ] fix the homing (the stepper direction are wrong the end stop are inerveted by default)
- [ ] fix the fan (the fan of the main board dont work neither the hotend fan)
- [ ] find the right step per mm for accuracy https://mpselectmini.com/extruder_calibration
- [ ] drill new holes in panel
- [ ] buy JST 3 connector and replace
- [ ] calmibrate extruder https://mpselectmini.com/extruder_calibration
- [ ] fix heat bed wire (tend to break) https://mpselectmini.com/mods#heat_bed_wiring use silicon cable instead of other
- [ ] copy the gloabl setting of the machine https://mpselectmini.com/users_manual_v2
- [ ] secure the washer under the carrier on the z rod https://www.reddit.com/r/MPSelectMiniOwners/comments/b0lq1l/zaxis_nut_broke_loose_maybe/
- [ ] replace the leadscrew https://hackaday.io/project/14823-monoprice-select-mini-maximum-3d-printer-mods/log/55525-upgrade-the-z-axis-with-a-nema17-stepper-and-tr8x8-leadscrew (must put a reductor because this is not as accurate as the original one)
