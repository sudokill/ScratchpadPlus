# ScratchpadPlus
A fork of Scratchpad with automatic creation of WPT

## Installation

The installation and usage are done in the same way as Scratchpad, see here: https://github.com/rkusa/dcs-scratchpad

## Launch
The software is opened by default via the shortcut: ctrl+shift+w

## Creation of WPT

When taking a coordinate, a new line starting with an asterisk appears: this is the line that will be inserted into the onboard computer. 
If you do not want to integrate a coordinate, simply delete the asterisk.

WARNING: if there are WPTs, they will be overwritten


#### F/A-18C: 

- in HSI>DATA, box "Precise" 
- at the AMPCD level: Display any page, EXCEPT the "TAC" page
- click on "Load all" and wait 


#### A10: 

- it is possible to name a WPT, to do this add the name just after the asterisk and before the first '|'.

    example: *|N 41°55.590'|E 044°10.440'|3140 => *T90|N 41°55.590'|E 044°10.440'|3140  => the WPT will be named "T90"

- go to the CDU screen, WPT Page
- click on "Load all" and wait

- Note: The A10 only allows for 50 WPTs to be entered, once this limit is reached, it is necessary to modify the already created WPTs. To indicate to ScratchpadPlus that it should modify the WPTs, insert a # at the first line of ScratchpadPlus. 

#### M2000:

- simply click on "Load all"
    

#### F-16C: 

- simply click on "Load all"

##
NB : if you add a coordinate in scratchpad and you have already inserted the others, all the coordinates will be reinserted into the onboard computer, so you must either erase the previous coordinates, or remove the asterisk


#### F-15E:

Since there is no next waypoint function on the F-15E, we must load all the waypoints at once using their respective waypoint numbers.

- Add all the waypoints for the route you want to enter. To specify target points, add a period (`.`) after the appropriate waypoint number(s) in the text box (example: `*|N 41°55.590'|E 044°10.440'|3140|5.` means that waypoint 5 will be a target point).

- Click "Load all" and the waypoints will be entered and configured as the appropriate type into route B.

Note that since we can't tell if any previously entered waypoint is a steerpoint or a target point, a longer sequence of key presses is used to guarantee we get the desired type of waypoint.

