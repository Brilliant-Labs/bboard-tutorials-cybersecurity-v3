# Activity 1

# Part 1 - Micro:bit Activity: Welcome to my City

The micro:bit is a powerful micro controller and you will have the chance to do some coding activities that will give you a better understanding of how to protect yourself and how the world of cyber security works. We will walk you through this and you can also give students time to explore and try to create their own programs. This activity will allow students to create a light-up poster to display their community's name.
They can take the name of their community or start thinking of a name they would like to use
for building their smart community later in the other activities.

# Step 1 : plug in the USB from the Micro:bit into your pc/laptop
<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

# Step 2 : Display your comunity name

1. In the ``||Basic:Basic||`` bar click and drag the **show icon** block and change it from **heart to happy** (1st row, last one)

2. In the ``||Basic:Basic||`` tab click and drag the ``||Basic:show string "hello"||`` block into the forever block and change it to ``||basic:show string "hackerville"||``


```blocks
basic.forever(function () {
    basic.showString("Hackerville")
})
```

# Explanation

The forever block executes the code permanently, i.e. without stopping. By placing the show string block inside the forever block, our community name will scroll on the screen without stopping.

In contrast, if we had placed the show string block inside the on start block, our community
name would have scrolled once and the code execution would end immediately after displaying the name on the screen.

The choice of the on start block or the forever block is a personal choice depending on the
objective.

