# **Activity 3**

# Part 1 - Activity with the micro:bit: Running a servo motor

The micro:bit is a powerful micro controller and you will have the chance to do some coding activities that will give you a better understanding of how to protect yourself and how the world of cyber security works. We will walk you through this and you can also give students time to explore and try to create their own programs. This activity will allow students to create a light-up poster to display their community's name.
They can take the name of their community or start thinking of a name they would like to use
for building their smart community later in the other activities.


# Step 1 : plug in the mircobit into your pc and you Bboard

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png) 

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG)

# Step 2 : plug in your servo motor

<!-- https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_3/servoPlugIn.png -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_3/servoPlugIn.png "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_3/servo_in%20board.JPG -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_3/servo_in%20board.JPG)


# Step 3 : coding your servo motor 

1. In the ``||input:input||`` tab drag the ``||input:on button A pressed||`` to your work space

2. In the ``||advanced:advanced||`` tab find the ``||pins:pins||`` tab for ``||pins:servo write pin P0 to 180||``

3. In the ``||input:input||`` tab drag the ``||input:on button A pressed||`` to your work space and change it from A to B

4. duplucate the block from step 3 part 2 and change the number from 180 to 0 and drag it in the ``||input:on button B pressed||``

```blocks
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 180)
})
input.onButtonPressed(Button.B, function () {
    pins.servoWritePin(AnalogPin.P0, 0)
})
basic.showIcon(IconNames.Happy)
```
# Explanation 
The code we have developed allows for 2 possibilities. First, when we press button A, the servo motor will turn 180 degrees.

Secondly, when we press button B, the servo motor will turn in the opposite direction.

