# **Activity 4**

# Part 1 - Activity with the micro:bit: The Temperature Sensor

This activity will allow students to program and operate a temperature sensor using a
micro:bit.

# Step 1 : plug in the microbit to the to your pc and the Bboard 

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")
---
<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)
---
<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png) 
## Step 2 : temperture gage 
1. open up the [basic] tag and drag in the [show string "Hello"] and drag it into the [forever] block
2. in the [Input] scroll down andd find the [temperatue (°c)] and click and drag it into the [show string "Hello"] block
3. in the [input] find the [pause (ms) 100] block and change the **100 to 1000**

```
basic.showIcon(IconNames.Yes)
basic.forever(function () {
    basic.showString("" + (input.temperature()))
    basic.pause(1000)
})
```
