# Projet / Partie 6



## Partie 6:
- Ensemble

## Atmega
Vous avez l'équivalent d'un Arduino Nano en main, le nom exact de votre circuit est le AtMega328P. Le programme installer sur les headers est le Bootloader Atmel-ICE via le programmeur Atmel de Microchip.

À partir de ce moment, vous pouvez installer le bootloader et le programme que vous voulez. Le AtMega328P est un module avec moins de mémoire et moins de GPIO que le Arduino Mega dans le cours de Microcontrôleur 1/2 et Communication Numériques. Cependant, les programmes sont compatibles si la mémoire et les GPIOs le permettre.

Pour la section final, aller prendre une strip de DELs/LEDs de 15.

Voici le code à installer:


```
#include <Arduino.h>
#include <FastLED.h>

#define NUM_LEDS 10

#ifndef PIN_DATA
#define PIN_DATA 3
#endif  // PIN_DATA


// Define the array of leds
CRGB leds[NUM_LEDS];
int pos = 0;

void setup() {
    Serial.begin(115200);
    Serial.println("Compteur version code!");
    FastLED.addLeds<NEOPIXEL, PIN_DATA>(leds, NUM_LEDS); 
}

void loop() {
  for (int i = 0; i < NUM_LEDS; ++i) {
    if (i == pos)
    {
      leds[i] = CRGB::Green;
    }
    else
    {
      leds[i] = CRGB::Black;
    }
    
  }
  pos += 1;
  if (pos >= NUM_LEDS)
  {
    pos = 0;
  }
  FastLED.show();
  delay(250);
}
```

Pour le branchement:

```
// Vin <--> Vcc
// DataIn <--> 3
// GND <--> GND

```



> $\color{gray}{\text{MANIPULATION}}$ **Simuler le compteur avec un système numérique**
>
> Installer la librairie `FastLed` avant d'installer le programme.
> 
> Brancher la pin de data des DEL sur 3.
>
> Installer le programme.
>



> $\color{darkred}{\text{À VÉRIFIER}}$ **Faire le compteur**
>
> Valider avec l'enseignant le `nouveau` compteur
> 

> $\color{darkgreen}{\text{À NOTER}}$ **Partie 6**
>
> Répondre si vous voulez à la partie 6. Projet fini!
> 
> 