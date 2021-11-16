

# Activité 1
# Bienvenue dans ma communauté

# Étape 1 : Branchez le câble USB du Microbit dans votre port USB

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

# Étape 2 : affichage le Nom de ton  ccommunauté
1. Dans la barre [de base], cliquez et faites glisser le bloc d'icônes d'affichage et changez-le de cœur en heureux (1ère rangée, dernière)
2. Dans l'onglet [de base], cliquez et faites glisser le bloc show string "hello" dans le bloc forever
3. Dans l'onglet [avancé], cliquez sur le bouton de texte, faites glisser le bloc "" et placez-le au-dessus de la partie hello du bloc show string et remplacez le texte par le nom de votre communauté

```
basic.showIcon(IconNames.Happy)
basic.forever(function () {
    basic.showString("My City")
})
```
