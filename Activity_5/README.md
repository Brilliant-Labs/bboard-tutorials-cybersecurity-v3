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
1. in the ``||radio:radio||`` tab find the block ``||radio:radio set group 1||`` into the ``||basic:on start||`` block
2. in the ``||input:input||`` tab drag the ``||basic:forever||`` block and drag the ``||radio:radio send string ""||`` block and change the "" to welcome
3. in the ``||radio:radio||`` tab drag the ``||radio:on radio received receivedString||`` and drag the ``||show string "hello"||`` blocks and change the "hello" to the "receivedString"

```blocks
radio.onReceivedString(function (receivedString) {
    basic.showString(receivedString)
})
radio.setGroup(1)
basic.forever(function () {
    basic.showString("Welcome")
})
```
# Explanation
By telling the microbit to listen on channel 1, this will affect all the microbits that will be on the same channel. Subsequently, we transmit a message on channel 1. In this case : Welcome!
The next block will receive the signal that has been sent and display it. This will affect all the
microbits that are on the same channel. Thus, all students should see the same message
scrolling by when one group press the A button.
