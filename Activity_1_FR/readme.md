

# Activité 1
# Partie 1 - Activité de programmation d’un micro:bit : Bienvenue dans ma ville...

Cette activité permettra aux élèves de créer une affiche lumineuse pour afficher le nom de leur communauté. Ils peuvent prendre le nom de leur communauté ou commencer à réfléchir à un nom qu’ils aimeraient utiliser pour la construction de leur communauté intelligente un peu plus loin dans les autres activités.

# Étape 1 : Branchez le câble USB du Microbit dans votre port USB

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

# Étape 2 : affichage le Nom de ton  ccommunauté
1. Dans la barre ``||basic:Basic||``, cliquez et faites glisser le bloc d'icônes d'affichage et changez-le de cœur en heureux (1ère rangée, dernière)
2. Dans l'onglet ``||Basic:Basic||``, cliquez et faites glisser le bloc ``||Basic:show string "hello"||`` dans le bloc forever
3. change le bloc ``||Basic:show string "hello"||``, au nom de votre communauté

```blocks
basic.forever(function () {
    basic.showString("Hackerville")
})
```

# Explication du code
Le bloc toujours exécute le code de manière permanente, c’est-à-dire sans s’arrêter. En plaçant le bloc afficher texte à l’intérieur du bloc toujours, le nom de notre communauté défilera à
l’écran sans jamais s’arrêter.

À l’opposé, si nous avions placé le bloc afficher texte dans le bloc au démarrage, le nom de notre communauté aurait défilé une fois et l’exécution du code se terminerait immédiatement après avoir fait
afficher le nom à l’écran.

Le choix du bloc au démarrage ou bien du bloc toujours reste un choix personnel en fonction de l’objectif recherché.
