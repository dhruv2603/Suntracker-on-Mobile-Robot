# Suntracker_rocker-bogie
IV Labs summer project in which solar panels which always points towards sun is attached upon an all terrain robot base(Rocker-Bogie mechanism) that is controlled remotely by Bluetooth joystick app.
Codes for suntracker and controlling of rocker bogie by bluetooth are seperated.


*Note: bluetooth code is for app named 'joystick Bluetooth commander' for other apps modify it according to the output of the said app*

## Softwares Required
  * [Arduino IDE](https://www.arduino.cc/en/Main/Software)
  * [Joystick Bluetooth Commander App](https://play.google.com/store/apps/details?id=org.projectproto.btjoystick&hl=en)
  
## Theory

  ### Rocker-Bogie Mechanism
    X and Y values are used to have precise control of Left Hand Side(LHS) and Right Hand Side(RHS) motors. Simply,
    if Y is +ve the LHS motors will have Y+X speed and RHS motor will have Y-X speed. If Y is -ve then LHS motors 
    will have Y-X speed and RHS motors will have Y+X speed. Direction of rotation will be decided according to the
    signage of values of Y+X and Y-X in both the cases. This will the bot to move according to the position of 
    joystick on screen. It i seasy to figure out how this can take care of all possible cases of movement one 
    might require fromm bot.
    
  ### Suntracker
    In this case 4 ldrs are kept along +ve and -ve X-Y axis. Values obtained from ldrs along X-axis and Y-axis are
    compared and then the whole apparatus is moved with the help of two servos such that the difference between 
    them becomes less than 50. After every comparisions solar panels moves by 1 deg reducing the differnce between 
    ldrs readings.
    
## Highlighting features
  * The vehicle can traverse slopes of upto 45&#176; gradient
  * Obstacles of height 15cm can be overcome by the vehicle
  * Suntracker increases energy trapping efficiency by 38.96%.

## Paper
- [__Suntracker on Rocker-Bogie Mechanism__](https://doi.org/10.1007/978-981-15-3639-7_86), Murarka,S. et al, Kalamkar, V., Monkova, K. (eds) Advances in Mechanical Engineering. Lecture Notes in Mechanical Engineering. Springer, Singapore, 2020.
## Credits
  ### Team Members
  * Aditya Wadichar
  * Shravar Tanawde
  * Shruti Murarka
  * Abhijit Rehpade
  * Dhruv Agrawal
  ### Mentors
  * Mohammad Saad
  * Sharan Bajjuri
  ### Special Thanks
  Dr. Shital Chiddarwar



<img src="https://github.com/Oopsydoopsy/Suntracker_rocker-bogie/blob/master/Suntracker.jpg">
