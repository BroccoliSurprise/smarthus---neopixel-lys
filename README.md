# Intro til NeoPixel-lys

## Steg 1 - Hva er NeoPixler? @showdialog

Fine fine lys!

![animert gif av neopixelring](https://d14xnrffmhx4ml.cloudfront.net/1660675041/smarthus-veiledning-neopixelring.gif)

Inni hvert piksel er en mikroprosessor som kan styre farge og lysstyrke. 
Med riktige kommandoer går det an å lage vakre fargemønstre.



## Steg 2 -  Trekk ut USB-ledningen før du begynner å koble! @showdialog
**Viktig! Les dette før du begynner**  

Utstyret kan bli ødelagt om ledningene sklir eller kortslutter, så vær **helt** sikker på at det ikke er strøm i systemet når du skal koble til eller fra noe.

## Steg 3 -  Hvordan koble lysene til micro:biten 

![bilde av ledninger koblet på microbit](https://d14xnrffmhx4ml.cloudfront.net/1660675040/smarthus-veiledning-neopixel-ledninger.jpg)

Fra høyre til venstre skal det være svart på **GND**, rød på **3V**, og så hvit på **2**.


## Steg 4 -  Last ned koden

Last ned eksempel-programmet til micro:biten og sjekk om det blir liv i lysene.

```template
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
```

## Steg 5 - Flott! 

Hvis det ble lys: Hurra! Prøv å endre eksempel-programmet og se om du får til å endre fargen på lysene.


## Steg 6 - Analyse av koden @showdialog

Før vi fortsetter kan det være greit å vite hva programmet gjør:

micro:biten vet ikke av seg selv at vi har koblet LEDlys til den, vi må fortelle den det med kode.

I den første blokken lager vi en variabel som heter "strip", som forteller micro:biten hvilken utgang signalene skal sendes til (P2), hvor mange lys som er koblet i ledningen (5), og hvilken type lys-signaler som skal sendes (RGB).

Når vi har gjort det, kan vi kjøre NeoPixel-kommandoer fra menyen og si at de skal gjelde på lyslenken som heter "strip".

Det ligger veldig mye avansert kode under panseret på disse blokkene, men vi trenger heldigvis ikke å vite alle detaljene for å kunne bruke de.


## Steg 7 -- Kule greier

<!---

// https://makecode.microbit.org/#tutorial:https://broccolisurprise.github.io/smarthus---neopixel-lys/

// Open this page at [https://broccolisurprise.github.io/smarthus---neopixel-lys/](https://broccolisurprise.github.io/smarthus---neopixel-lys/)

