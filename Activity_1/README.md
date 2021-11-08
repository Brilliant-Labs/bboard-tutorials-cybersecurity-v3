# Activity 1

# Step 1 : plug in the USB from the micro bit into your pc/laptop
<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")


# Step 2 : Display your comunity name

1. In the [basic] bar click and drag the **show icon** block and change it from **heart to happy** (1st row, last one)

2. In the [basic] tab click and drag the **show string "hello"** block into the forever block

3. In the [advanced] tab click the text button drag the **""** block and put it over top of the **hello part of the show string block** and change the text to the **name of you comunuity**

```
basic.showIcon(IconNames.Happy)
basic.forever(function () {
    basic.showString("My City")
})
```
