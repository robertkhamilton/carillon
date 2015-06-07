# carillon
Carillon Demo README.txt
by Rob Hamilton
https://ccrma.stanford.edu/~rob/carillon
@robertkhamilton
Updated 6.5.2015

----- OVERVIEW -----

Carillon is a real-time virtual instrument built using the Unreal Engine and designed to be used in live concert performances, such as it's May 30, 2015 premiere with the Stanford Laptop Orchestra at Stanford University's Bing Concert Hall. 

Carillon was designed to allow multiple performers to interact with a giant virtual Carillon across the network, controlling the motion of parts of the instrument that generate sound and music. The environment was designed to be used with an immersive head mounted display (HMD) like the Oculus Rift and a Leap Motion hand tracking sensor, though the demo can be used without the HMD. 

This demo build of Carillon was designed to allow users to experiment with some of the sound-generating interactions that are used in the full version of the software. Using their hands, players can select rings from the Carillon and set them spinning with gestures. As the rings spin on different axes, parameters of sound and music are changed in real time, creating a musical experience.

----- INSTALLATION -----

To run the Carillon demo, users must install drivers for the Leap Motion and Oculus Rift (if they are using those devices) and must install the Pure Data computer music system (a free/open-source download) as well as the Carillon executable itself. At this time the Carillon demo runs only on __Windows__ machines and requires at a minimum a 2GB video card.

CARILLON DEMO

1) Download the carillondemo.zip file from https://ccrma.stanford.edu/~rob/carillon/demo/carillondemo.zip

2) Unzip the package.

3) In the /demo folder there are two folders, one for the app itself (/demo/carillon) and one for the Pure Data patches (/demo/pd).

- PURE DATA

Pure Data is an open-source music programming language created by Miller Puckette, a professor at the University of California, San Diego. Pure Data can be downloaded for free and is required to run the sound engine for the Carillon demo.

- Download and install the "Pure-Data Extended" installer from http://puredata.info/downloads or http://puredata.info/downloads/pd-extended (make sure you select Pd-extended as this patch needs that version to run). At the time of this writing Pd-Extended version 0.43.4 was the latest version.


- LEAP MOTION

Make sure your Leap Motion drivers and installers are up-to-date. Instructions and downloads for the Leap Motion can be found on the Leap Motion website: https://www.leapmotion.com/

- OCULUS RIFT

Drivers and setup software for the Oculus Rift DK2 can be found at http://oculus.com/
This demo was not tested using a DK1.


----- STARTING THE DEMO -----

To start the Carillon demo, after installing the required software and drivers:

1) Launch Pure Data Extended and select the carilon.pd patch from the carillondemo.zip
DEMO CONTROLS, or double-click the carillon.pd patch to launch Pure Data (if your file associations are set to associate .pd files with Pure Data Extended). You should hear sound from the patch; if not please check the audio settings in Pure Data to make sure your computer's sound card is properly selected.

2) Launch the carillon.exe demo executable. This can be found at /demo/carillon/WindowsNoEditor/carillon.exe. An instance of the Carillon Unreal environment should open.

3) If you are using an Oculus Rift (DK2) HMD, press the "\" to turn on Oculus Rift mode. The environment should now be visible within the Oculus Rift.

4) If you are not using an Oculus Rift and you are using a Leap Motion in standard/facing-up mode, move your hands above the Leap to see your actor's hands move in the environment. NOTE: the Leap Motion must be plugged in before the demo is launched.

----- ACTIONS AND KEY BINDINGS -----

The following gestures and key bindings will allow you to interact with the Carillon demo. Please note standard A,S,D,W,SPACE,ARROW KEY first-person control mappings + mouse look will allow you to move your actor throughout the environment, even though th main view of Carillon is your view at the start of the game.

At the center of the Carillon are a large set of gears, those are the main focus of the demo. To your left, hovering close to your actor's head are a smaller set of rings that mirror the large rings. These are your control interface/HUD with which you will interact.

LEFT HAND GESTURES

- Swipe your hand from left to right to "expand" your HUD rings. You should see them move horizontally across your field of vision.

- Swipe your hand from right to left to "contract" your HUD rings.

- Place your hand over either one ring (if "expanded") or over all rings (if "contracted") to select the ring(s). Hold your hand there for one second to select the ring(s). If properly selected the ring(s) will turn red. Selected rings are now set to be controlled by swipes made with your right hand.

- To deselect a ring(s) place your hand again over the red ring(s) and hold for one second.

- To stop the selected ring(s) from rotating swipe your left hand away from your body.

RIGHT SWIPE GESTURES

- Swipe your hand from right to left to start the selected ring(s) spinning. This increases their yaw rotation. Swipe your hand from left to right to spin the ring(s) in the opposite direction.

- Swipe your hand away (or towards) your body to spin the selected ring(s) by increasing their pitch.

- Swipe your hand up or down in spin the selected ring(s) by increasing their roll.


KEYBOARD MAPPINGS

R - Re-orient your view if using the Oculus Rift.
G - Start the Carillon playing a bell sequence. The bell strikers can be see off to the left of your starting location, below your actor's location.

If not using the Leap Motion for gesture control, use the following key presses to interact with the Carillon:

Z - Expand/Contract the rings (same as left-hand horizontal swipe)
ALT+1,2,3,4,5,6 - Spin the rings (Same as right-hand swipes)
0 - Stop selected rings
U,I,O,P,[,] - Hold for one second to select/deselect a ring


ACKNOWLEDGEMENTS

Integration of the Leap Motion API within the Unreal Engine was done using the third-party event-driven Leap plugin for Unreal by getnamo: https://github.com/getnamo/leap-ue4

Open Sound Control integration within the Unreal Engine was done using monsieurgustav's UE4-OSC Unreal plugin: https://github.com/monsieurgustav/UE4-OSC


CONTACT

With any questions about the Carillon demo, please contact:

Rob Hamilton

twitter: @robertkhamilton
  email: rob@ccrma.stanford.edu
    web: http://robhamilton.io or https://ccrma.stanford.edu/~rob
