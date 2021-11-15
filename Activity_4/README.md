# **Activity 4**

# Step 1 : plug in the microbit to the to your pc and the Bboard 

plugged-in-microbit
<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

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
