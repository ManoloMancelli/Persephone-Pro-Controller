# Persephone Pro Controller V1 Assembly Guide

#
## This tutorial assumes that you already have a working HadesVR headset
#

## Required Parts and Tools

#### - All of the electronic parts included in the [BOM File](/Hardware/V1/BOM.md)
#### - Soldering Iron with fine tip
#### - Phillips Screwdriver
#### - Thin wire (I use Kynar)
#### - Double sided tape (Basic type. Nothing fancy)
#### - [3D printed parts](/Hardware/V1/STL)

## Main Frame Assembly

- ### 3D print the [Main Frame](/Hardware/V1/STL/Main%20Frame.stl)
![1](/Docs/V1/IMG/main%20frame%203d%20print.png)

- ### Assemble the [Button PCBs - 2pcs](/Hardware/V1/Electronics/Button%20PCB/Button%20PCB.zip)
![1](/Docs/V1/IMG/button%20pcb.jpeg)

- ### Cut off the battery connector if it comes with one
![1](/Docs/V1/IMG/battery_connector.jpeg)

- ### Solder the battery to the TP4056 PCB
![1](/Docs/V1/IMG/tp4056.jpeg)

- ### Apply small ammount of double sided tape to TP4056 and Battery
![1](/Docs/V1/IMG/tp4056_tape.jpeg)

- ### Stick the TP4056 and Battery into the Main Frame
![1](/Docs/V1/IMG/tp4056_frame.jpeg)

- ### Apply small ammount of double sided tape to Uno Mini, MPU-6500 and NRF24L01
![1](/Docs/V1/IMG/electronics_tape.jpeg)

- ### Stick the Uno Mini, MPU-6500 and NRF24L01 into the Main Frame
![1](/Docs/V1/IMG/electronics_frame.jpeg)

- ### Grab the Button PCBs and stick them over the plastic pillars
![1](/Docs/V1/IMG/button_pillars.jpeg)

- ### Melt the plastic pillars with your soldering iron
![1](/Docs/V1/IMG/pillars_melt.jpeg)

- ### Assemble the Joystick on top of the frame using self tapping screws
![1](/Docs/V1/IMG/joystick_frame.jpeg)

- ### Wire the MPU-6500
![1](/Docs/V1/IMG/mpu_wiring.png)

- ### Wire the NRF24L01
![1](/Docs/V1/IMG/nrf_wiring.png)

- ### Wire the Battery and TP4056
![1](/Docs/V1/IMG/battery_wiring.png)

- ### Wire the Joystick
![1](/Docs/V1/IMG/joystick_wiring.png)

- ### Wire the A/B Buttons
![1](/Docs/V1/IMG/ab_wiring.jpeg)

- ### It should now look more or less like this 
![1](/Docs/V1/IMG/frame_wiring_done.jpeg)

## Bumper Assembly
- ### 3D print the [Bumper](/Hardware/V1/STL/Bumper.stl)
![1](/Docs/V1/IMG/bumper_3d_print.png)

- ### Attach the Bumper to the Main Frame using two self-tapping screws
![1](/Docs/V1/IMG/bumper_assembly.jpeg)

## Finger Array Assembly

- ### 3D print the [Finger Array]()
![1](/Docs/V1/IMG/fingers_3d_print.png)

- ### 3D print the [Finger Buttons - 4pcs]()
![1](/Docs/V1/IMG/finger_buttons_3d_print.png)

- ### Assemble the [Button PCBs - 4pcs](/Hardware/V1/Electronics/Button%20PCB/Button%20PCB.zip)
![1](/Docs/V1/IMG/button%20pcb.jpeg)

- ### Place the Button PCBs over the plastic pillars
![1](/Docs/V1/IMG/finger_pillars.jpeg)

- ### Melt the plastic pillars with your soldering iron
![1](/Docs/V1/IMG/finger_pillars_melt.jpeg)

- ### Connect the Finger Array
![1](/Docs/V1/IMG/finger_wiring.png)

- ### Slide Finger Buttons between the hinge pieces
![1](/Docs/V1/IMG/hinges.jpeg)

- ### Insert pieces of filament into the hinges
![1](/Docs/V1/IMG/hinges_filament.jpeg)

- ### Melt filament ends with your soldering iron
![1](/Docs/V1/IMG/hinges_melt.jpeg)

- ### Attach the Finger Array to the Bumper
![1](/Docs/V1/IMG/finger_assembly.jpeg)

## Vive Tracker installation

- ### Screw the Vive Tracker onto the thread placed on the Bumper
![1](/Docs/V1/IMG/tracker.jpeg)

- ### Make sure that the Pogo Pins are in parallel to the Bumper
![1](/Docs/V1/IMG/pogo.jpeg)

## Firmware Installation

- #### Connect the Controller to your PC using Arduino UNO Mini USB port

- #### Open the [Firmware](/Software/Firmware/V1/Right_Controller) using Arduino IDE

- #### Select correct board and port inside Arduino IDE

- #### Upload the code

# Tracking Override

- #### This method is fully working in time of writing this tutorial (SteamVR build 21281713)

## PC Setup
- Install all of the latest Windows updates
- Install Steam Windows App
- Install SteamVR

## SteamVR Setup
- Connect your VR headset and make sure it works properly
- Go trough the Room Setup
- Connect the SteamVR Dongle and pair the tracker
- In SteamVR go to Devices -> Manage Trackers

![1](/Tutorials/SteamVR%20Tracking%20Override/img/0.png)

- Make sure your tracker has a green dot next to it

![1](/Tutorials/SteamVR%20Tracking%20Override/img/1.png)

- Click on the "Tracker Role" and select "Disabled"

![1](/Tutorials/SteamVR%20Tracking%20Override/img/2.png)

- Write down the tracker name

![1](/Tutorials/SteamVR%20Tracking%20Override/img/3.png)

## Tracking Override
- Close SteamVR if it's running
- Go to C:\Program Files (x86)\Steam\config
- Open steamvr.VRSETTINGS file with text editor (notepad is fine)
- Add below text to the file (make sure to put your tracker name which you've wrote down

```
   "TrackingOverrides" : {
      "/devices/htc/vive_trackerLHR-270B4DF0" : "/user/head"
   },
```

![1](/Tutorials/SteamVR%20Tracking%20Override/img/4.png)

- Save the file and close it
- Open SteamVR and enjoy Tracking Override