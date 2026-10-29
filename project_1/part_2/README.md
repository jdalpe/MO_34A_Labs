# Projet / Partie 2



## Partie 2:
- Assemblage manuelle de la moitié du PCB (Surface-mount)

## Intro

Pour la deuxième partie, souder l'ensemble des composants surface-mount restant, soit:


- C1, C4, C5, C6, C7
- U1
- D1
- R1, R2, R6, R8
- D3 (N'importe quelle couleur)


Préparer le restant du BOM avant de commencer votre travail


## Placement (MÊME section que Partie 1)

Nous avons des nouveaux types de composants dans ce circuits, aller regarder le schéma électrique dans `pinout` (arduino_nano).

#### Crystal (Through-hole)

Les crystaux ou oscillateurs sont des modules de quartz qui oscille à une fréquence défini. Ces 2 modèles sont respectivement de 12MHz et 16Mhz. Ils sont toujours accompagné de condensateurs de 22pF pour stabiliser l'horloge. À noter que ce sont des `crystaux`, des `oscillateurs` sont très similaire, mais les condensateurs sont à l'intérieur du module.

Il n'y a pas de polarité, mais attendez à la partie 3 pour le souder.

#### Diode simple (Surface-mount)

Il y a 2 diodes, utiliser le schéma électrique pour voir l'orientation. Comme les DELs/LEDs, ils ont une indicateur via une ligne, mais utilisé votre multimètre en mode `diode` pour voir l'orientation.

#### Point de diode

Il y a un pont de diode utiliser au niveau de l'entrée. Le but est de lire autant du analogique que de la tension numérique. Il est très important de bien le brancher. Regarder la datasheet `pont`. Le pont peut être placer en 2 orientations:

- ~~ <--> +-
- -+ <--> ~~


La meilleur façon est d'identifier + et -. Regarder dans quelle directions vont les diodes et avec votre multimètre en mode `diode`, vous pourrez voir comment le brancher.

**FAITES TRÈS ATTENTION, le point à l'envers peut court-circuité votre PCB en entier**

#### USB-C

Le port USB-C est quasiment impossible à faire à la souduire conventionnel, les pointes ne peuvent pas souder les pâtes sans brûler la section en plastique, bien suivre les instructions de l'enseignant pour ce composant en particulier.

#### Bornier à vis
Les borniers sont assez gros, assurez-vous d'aligner le tout pour avoir des connecteurs droits.

#### AtMega, Régulateur et CH340
Les nouveaux modules de type `U` sont plus nombreux que le compteur. Chacun est essentiel au fonctionnement, mais voici le rôle de chacun.

- AtMega: Il s'agit d'un AtMega328P, le microcontrôlleur utilisé dans les Arduino Nano, la documentation se trouve dans datasheet
- CH340G: Il s'agit du module en charge de la communication (et programmation) du AtMega. Il est essentiel pour programmer, mais pour pour executer le programme.
- Régulateur: Essentiel si on utilise une alimentation externe autre que le USB-C, il fourni jusqu'à 800mA.


# Évaluation


> $\color{darkred}{\text{À VÉRIFIER}}$ **Eval**
>
> Montrer à l'enseignant la soudure sans pâte (Aucun test requis)
> 
> 


> $\color{darkgreen}{\text{À NOTER}}$ **Partie 2**
>
> Prendre une photo de votre PCB à moitié rempli et ajouter la photo dans le rapport
> 
> 