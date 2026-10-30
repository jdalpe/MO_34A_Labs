# Projet / Partie 4



## Partie 4:
- Partie Through-hole essentielle (2/3)

## ALIMENTATION

Souder simplement `J3`,`C8` et `C9` 

L'alimentation passe par un pont de diode, le but d'un pont de diode est de redresser et rectifier la tension pour supporter plusieurs entrées: Plus grand voltage, signal inversé, AC, ...

Ce module est limité et fonctionne exclusivement en DC, le tout peut être alimenté avec une tension de 12V pour avoir un 5V à la sortie et pour le AtMega. 

Le tout fonctionne cependant en tension inversé. (Vin +-**PAS LE VOUT5V**)

> $\color{gray}{\text{MANIPULATION}}$ **Envoyer une tension positive et negative**
>
> Avec le bloc d'alimentation (9V, 0.3A), envoyer une tension par le connecteur `J3`. Sortir la valeur à l'oscilloscope du 5v (OUT)G (Mesure avec des pinces ou un fil, n'installer pas maintenant le bornier)
>
> Inverser les fils du bloc d'alimentation et prendre aussi la mesure sur l'oscilloscope. (2 canaux pour comparer avec la lecture de la tension visible)
>





> $\color{darkgreen}{\text{À NOTER}}$ **Partie 4**
>
> Prendre les analyses de votre oscilloscope et sauvegarder l'image dans votre rapport
> 
> 

> $\color{darkred}{\text{À VÉRIFIER}}$ **Faire valider les étapes suivantes en classe**
>
> Valider avec l'enseignant:
> - Application de tension positive
> - Application de tension négative
> **NOTE: Appliquer uniquement 9V et 0.3A, si votre pont de diode est mal installé, on ne veut pas endommager le ATMega**
> 
> 