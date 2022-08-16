# Intro til NeoPixel-lys

## Hva er NeoPixler? @unplugged

Fine fine lys!

![picture of neopixels](/.docs/static/tutorials/neopixelring.gif)

Inni hvert piksel er en mikroprosessor som kan styre farge og lysstyrke. 
Med riktige kommandoer går det an å lage vakre fargemønstre.

```template
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
```

## Hvordan koble lysene til micro:biten @showhint

![picture of connecting wires](/.docs/static/tutorials/neopixelwires.jpg)

## Last ned koden

Last ned koden til micro:biten og sjekk om det blir liv i lysene.

## Flott! @showhint
<!---

// https://makecode.microbit.org/#tutorial:https://broccolisurprise.github.io/smarthus---neopixel-lys/

// Open this page at [https://broccolisurprise.github.io/smarthus---neopixel-lys/](https://broccolisurprise.github.io/smarthus---neopixel-lys/)

