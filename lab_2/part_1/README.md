# Laboratoire 2 / Partie 1



## Partie 1:
- Désoudure


# But de l'exercise

Déssouder un circuit est beaucoup plus rare comme manipulation que l'inverse. En effet, un technicien/ne aura un ratio de 1:10 ou même plus pour effectuer une réparation selon le domaine.

En tant que technicien/ne dans une entreprise, le but est de construire un maximum de circuits avec un taux d'échec minimal (Appeler `yield`). 

Ce laboratoire va s'assurer de pratiquer pour les cas suivants:

- Un PCB a été en production trop tôt et il y a des problèmes.
- Faire un plan (`defect plan`) pour s'assurer du suivi.
- Vous voulez changer de composants sur une carte
	- Cas `Homemade`:
		- Votre PS5 fonctionne, mais pas votre port HDMI?
		- Votre AtMega a été survolté et il est décédé?

# Enlever des composants

Voici un exemple sur un composant à 2 pin Surface-Mount 
TBD tresse

**Diode, DEL, Résistance, Condensateur**

- Voici un exemple avec la résistance `R2`

![](gui/r2.jpg)

- Toujours commencer par appliquer le flux
	- En mettre pour couvrir les 2 pads

![](gui/r2_flux.jpg)

- Préparer votre pointe
![](gui/seasoned.jpg)

- Pour des composants de ce type, prenez assez d'étain pour couvrir les 2 pad de soudure
![](gui/r2_over.jpg)

- Positionner votre pointe pour qu'elle connecte au 2 pads en même temps

- Une fois l'étain main, balayer le composant et celui-ci va coller à votre pointe. 

- Refroidir dans l'éponge (Enlever le composant ET enlever l'extra)

- Tresse a dessouder pour l'exces

- Laver le tout avec de l'alcool (Avec brosse à dent, lingette ou papier)
![](gui/r2_remove.jpg)



------


Voici un exemple sur un composant à plusieurs pin Surface-Mount (Avec pistolet à air chaud) **Commencer le travail à votre station, mais aller à la station des pistolets à air chaud pour enlever votre pièce**

**SOIC, L-Lead, J-Lead**

- Voici un exemple avec le IC U4
![](gui/select_soic.jpg)

- Toujours commencer par appliquer le flux
![](gui/flux_soic.jpg)

- Préparer votre pointe
![](gui/seasoned.jpg)

- Soudure en surplus

- Tresse a dessouder pour l'exces
![](gui/heat_solder_soic.jpg)

- Utiliser le pistolet thermique et placer vos pinces pour pouvoir retirer le composant (idéalement, ne pas appliquer de force sur les pin, juste le contenant noir)
![](gui/tweezer_soic.jpg)
![](gui/heated_soic.jpg)


- Une fois que les broches brillent (Étain malléable), appliquer une force pour enlever le composant. Commencer par bouger latéralement avant de tirer vers le haut
![](gui/remove_soic2.jpg)
![](gui/remove_soic3.jpg)

------

Voici un exemple sur un composant de type Through-hole
(Avec pistolet pour dessouder)

#### Pistolet a dessouder

- Enlever le cap bleu
![](gui/desolder_tip.jpg)

- Insérer l'embout
![](gui/desolder_tip2.jpg)
![](gui/desolder_tip3.jpg)

- Démarrer le tout à votre temperature désiré (Autour de 680 est un bon début)

- Si la pointe se met à fumer un peu, c'est que la buse est neuve, placer la pointe du pistolet sur l'éponge un moment
	- Éteindre et le rallumer au moment de l'extraction

**DIP, Headers, Connecteurs**

- Voici un exemple avec la DEL D51
![](gui/del.jpg)

- Toujours commencer par appliquer le flux
![](gui/del_flux.jpg)

- Soudure en surplus

- Avec des pinces de précision `tweezer`, tenir la pièce

- Appliquer le bec du pistolet
![](gui/del_heated.jpg)

- Au moment ou l'étain devient mou, activer la suction et tirer avec vos pinces
![](gui/del_after.jpg)

- S'il reste quelques traces de soudure, passer un coup de tresse

------

Voici un exemple sur un composant de type Through-hole
(Avec pompe manuelle)
![](gui/pump.jpg)

**DIP, Headers, Connecteurs**

- Voici un exemple avec le condensateur C13
![](gui/cap.jpg)
![](gui/cap_2.jpg)


- Toujours commencer par appliquer le flux

- Préparer votre pointe de fer à souder (`seasoned`) et vidé votre pompe manuelle

- Ajouter un peu d'étain sur la broche à enlever

- Avec des pinces de précision `tweezer`, tenir la pièce

- Appliquer le fer à souder

- Au moment ou l'étain devient mou, tirer sur la pièce

- Pour laver la trace au moment ou l'étain devient mou, approcher votre pompe et aspirer
![](gui/cap_manual.jpg)

- S'il reste quelques traces, passer un coup de tresse

### Pourquoi on réapplique de la soudure?

Un peu comme le `seasoning` de la pointe à souder, il faut avoir une surface de travail. L'étain utiliser par le fabricant de la carte PCB n'est pas exactement le même que le notre. De plus, avec le temps, il y a des impuretés sur la soudure. 

En placer en surplus va s'assurer de `laver` les impuretés, de contrôle la composition chimique de notre étain et de contrôler la température en stressant le moins possible le pad ou la broche connectée.

De plus, avec plus de soudures, on peut profiter d'un effet de suction d'un coup via une tresse, un pistolet ou une pompe. 


> $\color{gray}{\text{MANIPULATION}}$ **Clean up**
>
> L'enseignant passera à votre station et vous donnera 4 composants à enlever
>
> Utiliser la méthode qui vous semble la meilleure pour vos pièces électroniques
>
> La survie des composants n'est pas importante ici, c'est le PCB qui nous importe
>


> $\color{darkred}{\text{À VÉRIFIER}}$ **Clean up eval**
>
> Montrer à l'enseignant l'emplacement des 4 composants enlevés
> 
> 