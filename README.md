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

## Trekk ut USB-ledningen før du begynner å koble! @unplugged

Utstyret kan bli ødelagt om ledningene sklir eller kortslutter, så vær helt sikker på at det ikke er strøm i systemet når du skal koble til eller fra noe.

## Hvordan koble lysene til micro:biten 

![picture of connecting wires](/.docs/static/tutorials/neopixel-ledninger.jpg)

Fra høyre til venstre skal det være svart, rød, og så hvit.


## Last ned koden

Last ned koden til micro:biten og sjekk om det blir liv i lysene.

## Flott! 

Hvis det ble lys: Hurra! Se om du får til å skifte fargen på lyset.

## Analyse av koden

Før vi fortsetter kan det være greit å vite hva programmet gjør:

micro:biten vet ikke av seg selv at vi har koblet LEDlys til den, vi må fortelle den det med kode.

I den første blokken lager vi en variabel som heter "strip", som forteller micro:biten hvilken utgang signalene skal sendes til (P2), hvor mange lys som er koblet i ledningen (5), og hvilken type lys-signaler som skal sendes (RGB).

Når vi har gjort det, kan vi kjøre NeoPixel-kommandoer fra menyen og si at de skal gjelde på lyslenken som heter "strip".

Det ligger veldig mye avansert kode under panseret på disse blokkene, men vi trenger heldigvis ikke å vite alle detaljene for å kunne bruke de.

<!---

// https://makecode.microbit.org/#tutorial:https://broccolisurprise.github.io/smarthus---neopixel-lys/

// Open this page at [https://broccolisurprise.github.io/smarthus---neopixel-lys/](https://broccolisurprise.github.io/smarthus---neopixel-lys/)

