# Intro til NeoPixel-lys

```template
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
```

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

```blocks
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
```

## Steg 5 - Flott! 

Hvis det ble lys: Hurra! Prøv å endre eksempel-programmet og se om du får til å endre fargen på lysene.


## Steg 6 - Analyse av koden @showdialog

Før vi fortsetter kan det være greit å fortelle hvordan eksempel-programmet fungerer:

micro:biten skjønner ikke av seg selv at vi har koblet LEDlys til den, vi må gjøre den oppmerksom på dette med kode.

I den første blokken lager vi en variabel som får navnet "strip", som inneholder informasjonen micro:biten trenger: Hvilken utgang signalene skal sendes til (P2), hvor mange lys som er koblet i ledningen (5), og hvilken type lys-signaler som skal sendes (RGB).

Når vi har gjort det, kan vi kjøre NeoPixel-kommandoer fra menyen og si at de skal gjelde på lyslenken som heter "strip".


## Steg 7 -- Kule greier

I Neopixel-menyen til venstre finner du et knippe kommandoblokker som er fine å starte med. 

Oppdrag: Bruk noen minutter på å pusle sammen blokkene på ulike måter, og lag *kjempefine farger*

Når du føler deg fornøyd, kan du trykke på "Avslutt / Finish" for å gå tilbake til vanlig MakeCode med flere blokker.

```ghost
input.onButtonPressed(Button.A, function () {
    basic.pause(100)
})
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.clear()
strip.setPixelColor(0, neopixel.colors(NeoPixelColors.Red))
strip.setPixelColor(2, neopixel.colors(NeoPixelColors.Green))
strip.setPixelColor(4, neopixel.colors(NeoPixelColors.Yellow))
strip.show()
basic.pause(100)
strip.rotate(1)
strip.showRainbow(1, 360)
strip.setPixelColor(0, neopixel.colors(NeoPixelColors.Red))
strip.show()
basic.forever(function () {
})



