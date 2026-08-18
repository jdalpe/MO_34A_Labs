# Laboratoire 2 / Partie 1



## Partie 1:
- Désoudure


# But de l'exercise

Déssouder un circuit est beaucoup plus rare comme manipulation que l'inverse. En effet, un technicien/ne aura un ratio de 1:10 ou même plus pour effectuer une réparation selon le domaine.

En tant que technicien/ne dans une entreprise, le but est de construire un maximum de circuits avec un taux d'échec minimal (Appeler `yield`). 

Ce laboratoire s'assura de pratiquer pour les cas suivants:

- Un PCB a été en production trop tôt et il y a des problèmes.
- Faire un plan (`defect plan`) pour s'assurer du suivi.
- Vous voulez changer de composants sur une carte
	- Votre PS5 fonctionne, mais pas votre port HDMI?
	- Votre AtMega a été survolté et il est décédé?

# Enlever des composants

Voici un exemple sur un composant à 2 pin Surface-Mount 
TBD tresse

**Diode, DEL, Résistance, Condensateur**

- Toujours commencer par appliquer le flux
TBD image 1

- Préparer votre pointe
TBD image 2

- Pour des composants de ce type, prenez assez d'étain pour couvrir les 2 pad de soudure
TBD image 3

- Soudure en surplus
TBD image 4

- Tresse a dessouder pour l'exces
TBD image 5

- Laver le tout avec de l'alcool
TBD image 6


------


Voici un exemple sur un composant à plusieurs pin Surface-Mount (Sans pistolet thermique)
TBD tresse

**SOIC, L-Lead, J-Lead**

- Toujours commencer par appliquer le flux
TBD image 1

- Préparer votre pointe
TBD image 2

- Soudure en surplus
TBD image 3

- Tresse a dessouder pour l'exces
TBD image 4

- Laver le tout avec de l'alcool
TBD image 5

------

Voici un exemple sur un composant de type Through-hole
(Avec pistolet pour dessouder)
TBD image pistolet

**DIP, Headers, Connecteurs**

- Toujours commencer par appliquer le flux
TBD image 1

- Chauffer votre pistolet a dessoudure
TBD image 2

- Ajouter un peu d'étain sur la broche à enlever
TBD image 3

- Appliquer le bec du pistolet
TBD image 4

- Au moment ou l'étain devient mou, aspirer
TBD image 5

- S'il reste quelques traces, repeter
TBD image 6

------

Voici un exemple sur un composant de type Through-hole
(Avec pompe manuelle)
TBD image pompe

**DIP, Headers, Connecteurs**

- Toujours commencer par appliquer le flux
TBD image 1

- Préparer votre pointe de fer à souder (seasoned) et vidé votre pompe manuelle
TBD image 2

- Ajouter un peu d'étain sur la broche à enlever
TBD image 3

- Appliquer le fer à souder
TBD image 4

- Au moment ou l'étain devient mou, approcher votre pompe et aspirer
TBD image 5

- S'il reste quelques traces, repeter
TBD image 6

### Pourquoi on réapplique de la soudure?

Un peu comme le `seasoning` de la pointe à souder, il faut avoir une surface de travail. L'étain utiliser par le fabricant de la carte PCB n'est pas exactement le même que le notre. De plus, avec le temps, il y a des impuretés sur la soudure. 

En placer en surplus va s'assurer de `laver` les impuretés, de contrôle la composition chimique de notre étain et de contrôler la température en stressant le moins possible le pad ou la broche connectée.

De plus, avec plus de soudures, on peut profiter d'un effet de suction d'un coup via une tresse, un pistolet ou une pompe. 


> $\color{gray}{\text{MANIPULATION}}$ **Clean up**
>
> L'enseignant passera à votre station et vous donnera 4 composants à enlever
>
> La survie des composants n'est pas importante ici, c'est le PCB qui nous interesse
>


> $\color{darkred}{\text{À VÉRIFIER}}$ **Clean up eval**
>
> Montrer à l'enseignant l'emplacement des 4 composants enlevés
> 
> 