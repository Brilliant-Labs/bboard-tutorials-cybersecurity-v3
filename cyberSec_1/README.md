# IR Distance Click

![Magic](https://github.com/Brilliant-Labs/bboard-tuts/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Description

Using a combination of IR LEDs
and signal processing, this
distance sensor is great for
measuring objects or obstacles at 
distances between 10 and 150 cm!

![IR Distance Click](https://github.com/Brilliant-Labs/bboard-tuts/blob/master/ir-distance/ir-distance-click.jpg?raw=true "IR DISTANCE Click")

## Code Example

This example has the IR Distance Click plugged into to MikroBus #1 on the b.Board

```blocks

let Distance = 0
basic.forever(function () {
    Distance = IR_Distance.getDistance(clickBoardID.one)
    if (Distance < 30) {
        basic.showString("Near")
    } else {
        basic.showString("Far")
    }
    basic.pause(1000)
})
```

## Project Idea

THE MAGICIAN'S ASSISTANT

This sensor detects the presence of any object that is between 10 and 150 cm from its sensor. Create your own illusions by activating and deactivating a magic trick of your own design. Pull an object out of a hat and place it near the sensor to act as your own magical assistant! 

![Magic](https://github.com/Brilliant-Labs/bboard-tuts/blob/master/ir-distance/magicianGif.gif?raw=true "A magician's assistant")

