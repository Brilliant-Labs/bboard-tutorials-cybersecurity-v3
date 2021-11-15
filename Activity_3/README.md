# **Activity 3**

# Step 1 : plug in the mircobit into your pc and you Bboard

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png) 

# Step 2 : plug in your servo motor

<!-- https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_3/servoPlugIn.png -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_3/servoPlugIn.png "Click")

# Step 3 : coding your servo motor 

1. In the input tab drag the **on button A pressed** to your work space

2. In the advanced tab find the **servo write pin P0 to 180**

3. In the input tab drag the **on button A pressed** to your work space and change it from **A to B**eeee

4. In the input tab drag the the **servo write pin P0 to 180** and change it from **180 to 0** and drag it in the **on button B pressed**

```
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 180)
})
input.onButtonPressed(Button.B, function () {
    pins.servoWritePin(AnalogPin.P0, 0)
})
basic.showIcon(IconNames.Happy)
```
