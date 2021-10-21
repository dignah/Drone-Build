## **Open Skies Trainer Drone Build Guide** 

In this guide, we will document the equipment necessary to build a trainer drone using a KK flight controller. We will also provide the steps necessary to assembling the drone.

### **Equipment Required**
* Flight Controller - kk 2.1.5
* 4 Electronic Speed Controller - 30A
* 4 Brushless Motors - 2212-920kv
* 4 Propellers - 2ccw,2cw
* Radio receiver - Frsky X8R
* Radio Transmitter - Taranis X7 
* Frame - DJI F450
* 4 Jumper cables 

### **Configuration**
### Assembling 
### Transmitter Configuration
Transmitter used: Taranis QX7 
Inorder for this Tranmsitter to be used in a specific drone build ,you should create a file within specific transmitter .the following are the procedures on how to setup your transmitter 
* Switch on the Transmitter by pressing power button twice 
* Click on the menu button
* Use the Left button to move up and down select an empty number 
* Clic the left button to select the number
* select option "Create Model"
* Select model type if its Plane,Delta or MUlti 
* For my design i selected Multi meaning a multirotor drone 
* Assign Channels 
    Throttle - CH3
    Roll - CH1
    Pitch - CH2
    Yaw - CH4
* Click page buttom in the transmitter 
* Click enter to confirm 
* Click on the page to give the name that you want for your model 

### Binding 
* Binding process this is the process that enables transmitter and receiver to communicate ,through this communication you will have full control of your drone 
* Switch on the transimitter 
* select the model that you created before
* Click on the page section 
* Drop down to Channel Range section 
* Select "CH1-16"
* Drop down to Receiver NUmber written as "RxNum"
* Select Bind 
* You will hear a beep sound from the transmitter 
* switch on you drone while pressing the bind button on the receiver 
* when the transmitter and Receiver bind the receiver provides a green light indicating its already bind with the receiver
* Click the enter button on the transmitter and test to see if your drone is responding according to your transmitter stick movements 
### kk 2.1.5 Configuration 
1. Factory Reset
    Before putting any sort of configuration in the kk 2.1.5 flight controller the first thing is to erase all the data that may be contained in a particular flight controller before putting some new variables
2. Load Motor Layout 
    Click Load Motor layout 
    Select the layout according to your drone design e.g Quadcopter x mode 
    Click enter 
    click ok 
3. Accelerometer Calibration 
    From the kk flight controller menu 
    select Acc calibration 
    NB: make sure your drone is placed on the level surface then click Continue 
4. Misc Setting 
    Minimum Throttle 10
    Alarm 105 
5. PI Editor
   Roll(Aileron) 
   P-Gain  75
   P-Limit 50
   I-Gain  40
   I-Limit 20
   
   Pitch(Elevator)
   P-Gain  75
   P-Limit 50
   I-Gain  40
   I-Limit 20
   
   Yaw(Rudder)
   P-Gain  75
   P-Limit 20
   I-Gain  30
   I-Limit 10
   
   Throttle
   P-Gain  75
   P-Limit 20
   I-Gain  30
   I-Limit 10
6. Self Level Setting
    P Gain 70
    P Limit 20
7. Receiver Testing 
    Set all the receiver value to zero by adjusting     trim settings 
8. Mode Setting
    -Self -Level : AUX
    -Link Roll Pitch : Yes
    -Auto Disarm : Yes
    -Receiver : std 
    -Channel Map : No
    -Lost Mode Alarm : Yes 
9. Esc Throttle Calibration
    -Switch on the transmitter
    -Put the transmitter sticks on the maximum level 
    -Press the First and last button on the flight          controller
    -Switch on the Quadcopter ,
    -After the Quadcopter is on it will display this      message "Throttle Passing through"
    -move stick to the minimum position 
    -Then release the 1st and 4th Button 
10. Arming 
    To power on the motor switch the transmitter first then plug in the Lipo Battery to switch on the kk flight controller ,then press the throttle stick down to the right to switch on the aircraft.

