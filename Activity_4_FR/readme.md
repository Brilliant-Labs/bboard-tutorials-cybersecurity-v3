# Activité 4

# Partie 1 - Activité de programmation d’un micro:bit : Le capteur de température
Le micro:bit est un microcontrôleur simple et vous aurez la chance de faire des activités de codage qui vous permettront de mieux comprendre comment se protéger et du fonctionnement du monde de la cybersécurité. Nous vous accompagnerons avec ceci et vous pourrez aussi donner du temps aux élèves pour explorer et essayer de créer leurs propres programmes.

# Étape 1 : Branchez le câble USB du Microbit dans votre port USB et connectez le microbit au bboard et assurez-vous que l'alimentation est connectée

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

<!--https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG)

# Étape 2 : Indicateur de température
1. ouvrez la balise ``||basic||`` et faites glisser le ``||show string "Hello"||`` et faites-le glisser dans le bloc ``||forever||``
2. dans ``||basic||`` faites défiler vers le bas et recherchez la ``||temperatue (°c)||`` et cliquez et faites-la glisser dans le bloc ``||show string "Hello"||``
3. dans le ``||input||`` recherchez le bloc ``||pause (ms) 100||`` et changez le **100 en 1000**
```
basic.showIcon(IconNames.Yes)
basic.forever(function () {
    basic.showString("" + (input.temperature()))
    basic.pause(1000)
})
```
