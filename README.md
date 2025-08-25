# Bedslinger Idex Conversion

This is an idex conversion for the Ender3 and it's other clone incarnations.


## Parts of Note
The carriage mount is reversible on an mgn12H and the shroud has clearance to allow it to shift a little so you can balance the height of the toolheads. This makes it really easy to redesign this as needed for other hotends. 

## In Process notes and other issues
Currently I need to finish the fan shroud and cable chain setup but this uses mostly m3 heat inserts and socket head cap screws for just about everything. A couple M4's on the fan holders for the hotends/carriages but really the majority of this is using M3's I bought an assorted stainless metric bolt set for this and when I do the build log I'll go through it but it's fairly straightforward to get all of this going.

## Description

This kit assumes you have the dual-z axis kit from creality, as well as a linear rail an mgn12h 450mm to be precise. These 2 parts cost ~$50 at the time of writing but you will need a lot of other parts which will be listed. I also am using klipper for this project as this makes control with 2 boards reasonable.

## Printing Recommendations

* **Material:** PLA+, PETG, or ABS
* **Layer Height:** 0.16mm-0.2mm
* **Infill:** 20% (or specify if a different percentage is needed for strength)

## Parts

(Dual-Z Leadscrew mod)
(MGN12H 450mm length linear rail and 2 carriages)
3mm brass Hex Standoffs I got a variety pack but you need M3x6mm long ones
Assorted M3, M4, M5 brass heat inserts
Assorted M3, M4, M5 screws
A couple m4 nuts
M3 t-nuts
2 extra nema17 steppers
1 Extra control board (I used an skr mini e3 v2.0)
(Optional is another 24volt 250 watt psu, the dual z mod usually comes with a bracket, you can wire up to the old psu but I didn't want to redo my cable's)
gt2 idler pulley's, they come in 5mm bore and 3mm bore, tbh with what we are using them for you could get away with a 3mm bolt in a 5mm bore, I did and I'm printing fine. I actually realise writing this that I don't think the covers slot well for a 5mm bolt so I'll have to fix that, if you need to you should be able to in your slicer by adding a negative the side of your bolt of choice.
extra gt2 pulley, usually the cheap ones are 18teeth but printers like the ender3 have 20tooth ones, if you are harvesting another printer to user just keep that in mind.
5015 blower and axial fans, 2 of each
1 extra ender3 v2 hotend and extruder for mounting to the top of the frame.


## Assembly

I don't have full time to go over the entire assembly right now but I intend to once I finish the shrouds and cable chain mounts that are almost done, the covers and fan mounts have the insert holes for this included presently so you shouldn't need to reprint when those finish. I will give some rudimentary steps below.

Make sure you have the linear rail on first, it just makes life quite a bit easier.

### Carriages
The Carriages are reversible but they do need 6 M3 heat inserts per, in order to mount the hotend and the fans. You will want to install the standoffs so you can check that they are reasonable square to the face of the carriage.
Once those are cooled you can put them on the linear rail's loose, lower your z axis until one of the nozzles touches, try to get them both just barely touching the print surface, you can use the old paper shim trick to get a feel or just get both the nozzles touching and tighten, you just want to be careful not to get too much tilt in it to avoid dragging during printing. 
With that out of the way you should be able to mount the shroud's and then add the fans. 

### Gantry parts
The X gantry is actually super simple, the plates have a negative of the ender frame so after you remove the current x endstop you can just remove the nut's of each idler roller one at a time insert the hole for one of the plates and put the nut back on and you should have enough thread to fully get to the plastic lock portion of the nut. It will feel flimsy but once you add the braces it will stiffen up a lot, the left side has holes so you can use the old endstop holes to bolt through to add some rigidity. the right doesn't but it will be quite solid.

### Covers
In general just add heat inserts before trying to assemble anything, but the covers are the only not so obvious ones, they need 4 M3 heat inserts, 4 on the front 4 on the back, so that you can screw them in from the back of the gantry plates and then be able to screw in the ooze catch from the front. The other two at the top are for future expansions. Before you fasten these I would highly recommend putting the idler pulleys on loose to these covers and running belts loose so when you assemble you don't have to fish them around it's really rough.
Once you've run the belts you can tighten the covers and it should be fine so long as you don't unscrew the idlers or something.

### Final assembly of the gantry
Now take the belts and loop them around the carriage ears (there's one on each side) and zip tie them down, trim the ends.

### Electronics
You'll have to figure your wiring out for your specific board on your own, I don't have my klipper config included because it's not completed but you can lookup the generic idex config and your board to get yourself up and running.


## How to Contribute

This is an open-source project. If you have improvements or suggestions, you are welcome to fork this repository and submit a pull request.

## License

This project is licensed under the Creative Commons Attribution 4.0 International License.

[![License: CC BY 4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)

This means you are free to:

* **Share** — copy and redistribute the material in any medium or format
* **Adapt** — remix, transform, and build upon the material for any purpose, even commercially.

Under the following terms:

* **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

### How to Attribute This Work

Please attribute this work to **WrigglyTentacles** and provide a link back to this repository: `https://github.com/WrigglyTentacles/BedslingerIdex`
