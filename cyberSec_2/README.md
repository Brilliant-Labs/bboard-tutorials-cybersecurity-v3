# INTRO TO THE IR SENSE 3


![IR](https://github.com/Brilliant-Labs/bboard-tuts/blob/master/ir-sense-3/The-IR-sensor-operation-schematic.png?raw=true "How IR works")

## Description

This thermal imaging sensor can
detect environmental heat
changes up to 1m (100cm) away, even
through glass. Also, this sensor
can be used to detect humans as
they approach the area where the
sensor is located.

![IR SENSE 3 Click](https://github.com/Brilliant-Labs/bboard-tuts/blob/master/ir-sense-3/ir-sense-3-click.jpg?raw=true "IR SENSE 3 Click")

## Code Example

This example has the IR SENSE 3 Click plugged into to MikroBus #1 on the b.Board

```blocks

basic.forever(function () {
    if (IR_Sense_3.isHumanDetected(clickBoardID.one)) {
        basic.showIcon(IconNames.StickFigure)
        music.beginMelody(music.builtInMelody(Melodies.Entertainer), MelodyOptions.Once)
    } else {
        basic.showIcon(IconNames.No)
    }
})
```

## Project Idea

THE INVISIBLE TRIP WIRE

Detect someone approaching from one meter
away. Use this click to activate your design
or set an alarm. This is great for projects
that draw a lot of power and can be activated
when being observed and de-activated when
the room is empty. Pair this with the Record
and Play click to play a noise when someone
approaches for a good scare!

![TripWire](https://github.com/Brilliant-Labs/bboard-tuts/blob/master/ir-sense-3/tripwire.gif?raw=true "Invisible Trip wire")