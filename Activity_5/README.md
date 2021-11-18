# **Activity 5**

# Part 1 - Activity with the micro:bit: Bluetooth interconnection of micro:bits

This activity will allow students to interconnect the micro:bits together with the 2.4GHz signal

# step 1: plug in the microbit into the pc and your Bboard 

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")
---
<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)
---
<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG)
# Step 2: Radio Sinal 
1. in the [radio] tab find the block [radio set group 1] into the on [start] block
2. in the [input] tab drag the [forever] block and drag the **radio send string ""** block and change the **"" to welcome**
3. in the radio tab drag the [on radio received receivedString] and drag the [show string "hello"] blocks and change the ["hello"] to the "receivedString"

```
radio.onReceivedString(function (receivedString) {
    basic.showString(receivedString)
})
radio.setGroup(1)
basic.forever(function () {
    basic.showString("Welcome")
})
```
