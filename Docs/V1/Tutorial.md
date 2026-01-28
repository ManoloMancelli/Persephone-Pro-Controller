# Persephone Pro Controller V1 Assembly Guide

## This tutorial implies that you already have a working HadesVR headset

## Required Parts and Tools

#### - All of the electronic parts included in the [BOM File](/Hardware/V1/BOM.md)
#### - Soldering Iron with fine tip
#### - Phillips Screwdriver
#### - Thin wire (I use Kynar)
#### - Double sided tape (Basic type. Nothing fancy)
#### - [3D printed parts]()

## Main Frame Assembly

- ### 3D print the [Main Frame]()
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
![1](/Docs/V1/IMG/ab_wiring.png)

## Finger Array Assembly

- ### 3D print the [Finger Array]()
![1](/Docs/V1/IMG/fingers_3d_print.png)

- ### 3D print the [Finger Buttons - 4pcs]()
![1](/Docs/V1/IMG/finger_buttons_3d_print.png)

- ### Assemble the [Button PCBs - 4pcs](/Hardware/V1/Electronics/Button%20PCB/Button%20PCB.zip)
![1](/Docs/V1/IMG/button%20pcb.jpeg)

## Bumper Assembly
- ### 3D print the [Bumper]()
![1](/Docs/V1/IMG/bumper_3d_print.png)



## Component Wiring

### - Finger Array Wiring
![1](/Docs/V1/IMG/fingers_wiring.png)

## Firmware Installation

- ### Connect the Controller to your PC using Arduino UNO Mini USB port

- ### Open the [Firmware](/Software/Firmware/V1/Right_Controller) using Arduino IDE

- ### Select correct board and port inside Arduino IDE

- ### Upload the code