# CNC_6-axis_motion_control_docs
Documentation for construction of the CNC 6-axis motion controlled camera platform by DIW

## Why am I doing this?
This is my work to document what it takes to print, construct, wire, and configure the [CNC 6-axis motion controlled camera platform](https://www.thingiverse.com/thing:4652484) by **Do It Whenever**.

He has a few really intriguing videos on YT as well that walk through why he did it and what it can do.
* [The greatest DIY MOTION CONTROL camera rig EVER - allegedly](https://www.youtube.com/watch?v=WNtC9EkYCYQ)
* [If you have a 3D PRINTER - you can MAKE THIS motion controlled camera](https://www.youtube.com/watch?v=UMwUnzjZ8Ao)
* [The greatest DIY MOTION CONTROL camera rig EVER | Part 2](https://www.youtube.com/watch?v=kPe2O8CkQAY)

There are several pieces that will be needed in order to build this poject.  I will be constructing them as I go through it.  If you are looking at this on github, then you have all the work I've written as of this point.  I'll update sections as I have more information.
* Printed Parts BOM
* Mechanical and Electrical Hardware BOM
* Software
* The writeup below explaining how to put all this together

# 3D Printed Parts
Here is a link to the [BOM of 3d printed parts.](https://github.com/Lukens4242/CNC_6-axis_motion_control_docs/blob/main/BOM%203d%20printed%20parts.ods)

I organized things by several colors.  You will have the following that you can choose as you wish.  I color coded certain components to match up with the color of the release buttons caps, so less thinking was involved.  That is to say, I thought that pressing the blue release button and have it unlock the axis with the blue gears and components would be relatively intuitive.
* Base color
* Accent color
* Control Button Color #1
* Control Button Color #2
* Control Button Color #3
* Control Button Color #4
* Control Button Color #5 (for focus gear, I used black to keep any odd reflections from appearing in the images.)
* Control Button Color #6 (for zoom gear, I used black to keep any odd reflections from appearing in the images.)

# Mechanical and Electromechanical Hardware BOM
Here is a link to the [BOM of Hardware Components](https://github.com/Lukens4242/CNC_6-axis_motion_control_docs/blob/main/BOM%20Hardware.ods).

Note: I will be updating the small hardware section of this sheet as I consume components during the build.

# Software
You will need the following:
* [RPiOS or Ubuntu on a microSD card for a RPi](https://www.raspberrypi.com/software/)
* [Universal G-Code Sender](https://winder.github.io/ugs_website/)
* [GRBL Mega 5X fork](https://github.com/fra589/grbl-Mega-5X)

# Construction

Here are the colors I chose for things so that hopefully the images aren't too confusing.
* Base Color - Black
* Accent Color - Gold & Copper (I ran out of gold and had to sub copper for some parts)
* CBC1 (vertical arm movement) - Red
* CBC2 (horizontal arm movement) - Yellow
* CBC3 (cam tilt) - Blue
* CBC4 (cam pan) - Green
* CBC5 (focus)- black
* CBC6 (zoom)- black

For each subsection I will list the hardware needed and add that to the overall BOM.

## Slew Bearing

The slew bearing is made up of:
* Bearing Race Inner Bottom
* Bearing Race Inner Top
* Bearing Race Outer
* Nylon Spacer
* 24x rollers


I didn't have any nylon filament, so I printed the spacer out of PLA and sanded the various rubbing surfaces smooth.  I printed all of these at 35% grid infill with three exterior walls.  If I find that this doesn't work, I'll come back and let you know what I did to alleviate the situation.

Hardware needed:
* 8x M3x30 socket head cap screws
* 16x M3 washers
* 8x M3 nuts

The screws get two washers each put on them and then they come up from the bottom, with the nuts on top.  Four of the screw holes don't have the proper recesses for screws.

Top:
![Top](images/slew_bearing_top.jpg)

Bottom:
![Bottom](images/slew_bearing_bottom.jpg)

##Tripod Mounting Block
Now you can attach the tripod mounting block.

Hardware Needed:
* 8x M3x30 screws
* 8x M3 nuts

Be sure to line up the large hole in the slew bearing along with the tripod mounting block.  Shown below is the underside of the tripod mounting block along with the hole you need to make sure you align.

![mounting block](images/tripod_mount.jpg)


