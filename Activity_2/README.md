# **Activity 2**
 
# Part 1: Activity with the micro:bit: Make a Blixel light up

The micro:bit is a powerful micro controller and you will have the chance to do some coding activities that will give you a better understanding of how to protect yourself and how the world of cyber security works. We will walk you through this and you can also give students time to explore and try to create their own programs. This activity will allow students to create a light-up poster to display their community's name.
They can take the name of their community or start thinking of a name they would like to use
for building their smart community later in the other activities.

# Step 1 : plug in the USB from the micro bit into your pc/laptop

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")
---
<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

# Step 2 : conect the microbit into the bboard and make sure the power suply is conected
<!--https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png)

<!--https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG)

# Step 3 : once the microbit is conected 
1. Click the ``||Advanced||`` tab and find the BLixels tab
2. once in the ``||BLiXels||`` tab click and drag the **set all blixels to red** block and drag it into the for ever block
3. turn on the bboard with the switch at the side and see if the light are red
4. (if the Blixels are not red) repeat the Step 3 Once more

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(1).png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(1).png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(2).png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(2).png)
# Step 4 : if the light are red
1. under the ``||Variables:Variables||`` tab create a brand new variable called **password**
2. once you have set you brand new variable has been created drag the ``||Variables:Set password to 0||`` into the ``||basic:on start||`` block as well cick and drag from the ``||Basic:Basic||`` the ``||basic:show icon||`` and change it from the **heart to yes** (1st row, 3rd one)
3. ``||variables:set password to 0||`` block and change it to ``||variables:set password to 123456||``

# Step 5 : if every thing works 
1. from the ``||Logic:Logic||`` tab drag the ``||logic:if true then||`` block and hit the plus button it should now look like ``||logic:if true then else||``
2. grab the ``||Blixels:set all Blixels to red||`` and put it in the ``||logic:if true then||`` and put one into the ``||Logic:else||`` and change the one in the ``||Logic:if true then||`` to the color **green** (2nd row, 1st one) 
```blocks
let password = "123456"
basic.showIcon(IconNames.Yes)
basic.forever(function () {
    if (password == "123456") {
        BLiXel.showColour(0x00ff00)
    } else {
        BLiXel.showColour(0xff0000)
    }
))
```
# Explanation
We started by creating a variable named password and placed it in the block startup by assigning it the value 123456. This tells the micro:bit to create the variable and assign the text 123456 to it as soon as the micro:bit is started.

Afterwards, we inserted a little logic in the forever block in order to specify to the micro:bit what would happen if our variable did not have the same value as the password assigned to our logic. If the password of our variable password (which is created at startup) is equal to the text 123456, then the lights turn on green. Otherwise, the lights will turn red. Try changing the password in one place and see what happens.
