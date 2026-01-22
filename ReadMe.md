# The Robotic 'Surveillance Garbage Can' using a HandyBoard SBC - From 2009

This repo documents the evolution and development of a flip-up 'Surveillance Garbage Can'  robot based on a 6811 [HandyBoard SBC](http://handyboard.com) or this [link](https://www.cs.uml.edu/~fredm/handyboard.com/hb.html) and various LEGO Technic motors and related pieces. 
While this does not fall into my "1970s and 1980s retro-computing" camp it is getting there in terms of its age and antiquity given its 2000-era HandyBoard SBC.

<div style="text-align:center">
<img src="/Images/IMG_5064.JPG" alt="" style="width:auto; height:75%;">
</div>

## The Premise for the Build

The whimsical premise behind this project was to create a normal looking garbage can which would transform into one of the world’s "best security systems" by night. The idea was that that sonar and dual light sensors would rotate up from inside of the can and adaptively track an intruder's movement via rotating both the base of the can and its flip-up top. When an intruder was located then the Surveillance Garbage would  emit a “beep” from its computer controlled piezoelectric speaker, and track the location of the intruder using both ultra-sound and light sensing. 

The ultimate goal was to transform an ordinary $8 flip-top garbage can into a fully automated, robotic surveillance tracking device.

<div style="text-align:center">
<img src="/Images/IMG_4867.JPG" alt="" style="width:40%; height:auto;">    
<img src="/Images/IMG_5065.JPG" alt="" style="width:40%; height:auto;">
</div>

## Naming the Project

The names which were considered for the project were:

- The Surveillance Garbage Can
- The Spy Can
- The Garbulator
- Flip-Top Spy Cam
- The “Peek-A-Boo Can-Cam”

## Operation of the Surveillance Garbage Can

The can was rotated via a LEGO Technic controlled geared-down motor (internal to the can) that turned a rubber-tire wheel outside of the can:

<div style="text-align:center">
<img src="/Images/IMG_4995.JPG" alt="" style="width:75%; height:auto;">
</div>

<div style="text-align:center">
<img src="/Images/IMG_5051.JPG" alt="" style="width:75%; height:auto;">
</div>

<div style="text-align:center">
<img src="/Images/IMG_5027.JPG" alt="" style="width:75%; height:auto;">
</div>

The top flipped up and rotated via a smaller LEGO Technic controlled geared-down motor:

<div style="text-align:center">
<img src="/Images/IMG_5016.JPG" alt="" style="width:75%; height:auto;">
</div>

The sensors were mounted on the inner surface of the flip-up top of the can:

<div style="text-align:center">
<img src="/Images/IMG_5036.JPG" alt="" style="width:75%; height:auto;">
</div>

And the HandyBoard SBC was mounted on a metal platform inside of the can and above the interior motor assembly:

<div style="text-align:center">
<img src="/Images/IMG_5038.JPG" alt="" style="width:75%; height:auto;">
</div>

<div style="text-align:center">
<img src="/Images/IMG_5055.JPG" alt="" style="width:75%; height:auto;">
</div>

Everything was controlled by the 6811-based HandyBoard SBC and its associated [simple controller program](/Src/Robotic_Surveillance_Garbage_Can_Controller.ic) written in '[KISS Interactive C](https://en.wikipedia.org/wiki/Interactive_C)' (IC4). We programmed the HandyBoard so that the light sensors would rotate the can around in a circle while the sonar device would be used to “beep” at people if they came too close. 

<div style="text-align:center">
<img src="/Images/IMG_5007.JPG" alt="" style="width:75%; height:auto;">
</div>
