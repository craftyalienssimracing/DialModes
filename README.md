# DialModes
Enable dial modes on Fanatec wheels via SimHub control mapper

Problem: Mode dials are limited use on Fanatec (and many other wheels) due to how they are mappable.
Ascher Racing and Lovely Sim Racing has a nice implementation but that only works with the firmware on the Asher Racing wheels.

Required: 
* SimHub - (buy a licence, it is such an awesome app and great value)
* ControlMapper - Only tested using an Arduino (leo clone) bridge
* Fanatec Control Panel
* DDU - Vocore (or other) DDU (at least one) 

Optional:
* Lovely Dash - IMO the best DDU solution out there

How it works:
Create 24 FN Key Modifiers in SimHub Control mapper 

1-12 will be Left Dial Modes
13-24 will be RIght Dial Modes

Basically each of the Dials are mapped (using Constant option on the MSP Fanatec control panel) to 24 FN modifiers in SimHub control mapper. 
Then in combination with other keys provide 24x the mappable buttons on a wheel.

On the Formula and Porsche Rims I use the up/down toggles in combination with the modes to adjust whatever based on the mode is selected.

i.e. RIGHT MODE 6 (DASH MODE) + UP = LEFT MFM
     RIGHT MODE 7 (CHAT MODE) + UP = Chat Volume UP
     RIGHT MODE 7 (CHAT MODE) + BTN 1 = Chat Volume Mute

What is missing from this, is the ability to visually know what each mode is, this is where the Lovely Dash had a great solution (which I have been infulenced by). 

So using the DDU with SimHub / Lovely Dash is my solution, on one of the DDU (I have 2x4" and 1x4.3" on my SimRig), I have Lovely Flags and with a custom SimHub overlay added.
This overlay, shows what the current mode for each of the dials is. When changed there is an Alert which shows at a glance what the new mode is.

To achieve this needs some simple Javascript and a dash layout that can be used as the overlay.
