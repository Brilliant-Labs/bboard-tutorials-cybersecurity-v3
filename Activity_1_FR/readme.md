

# Activité 1
# Partie 1 - Activité de programmation d’un micro:bit : Bienvenue dans ma ville...

Cette activité permettra aux élèves de créer une affiche lumineuse pour afficher le nom de leur communauté. Ils peuvent prendre le nom de leur communauté ou commencer à réfléchir à un nom qu’ils aimeraient utiliser pour la construction de leur communauté intelligente un peu plus loin dans les autres activités.

# Étape 1 : Branchez le câble USB du Microbit dans votre port USB

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

# Étape 2 : affichage le Nom de ton  ccommunauté
1. Dans la barre [base], cliquez et faites glisser le bloc d'icônes d'affichage et changez-le de cœur en heureux (1ère rangée, dernière)
2. Dans l'onglet ``||base||``, cliquez et faites glisser le bloc show string "hello" dans le bloc forever
3. change le bloc ``|| base

```
basic.showIcon(IconNames.Happy)
basic.forever(function () {
    basic.showString("My City")
})
```
