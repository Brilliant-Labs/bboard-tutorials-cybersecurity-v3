# Activité 3

# Partie 1 - Activité de programmation d’un micro:bit : Faire tourner un servo moteur
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

# Étape 2 : branchez votre servomoteur
<!--https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_3/servoPlugIn.png -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_3/servoPlugIn.png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_3/servo_in%20board.JPG -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_3/servo_in%20board.JPG)

# Étape 3 : coder votre servomoteur
1. Dans l'onglet de ``||input:input||``, faites glisser ``||input:on button A pressed||`` vers votre espace de travail 
2. Dans l'onglet ``||advanced:advanced||``, recherchez la ``||servo write pin P0 to 180||`` dans ``||pins:pins||``
3. Dans l'onglet de ``||input:input||``, faites glisser ``||input:on button A pressed||`` vers votre espace de travail et modifiez-le de A à B
4. dupliquez le bloc de l'étape 3 partie 2 et changez le nombre de 180 à 0 et faites-le glisser dans le ``||input:on button B pressed||``

```blocks
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 180)
})
input.onButtonPressed(Button.B, function () {
    pins.servoWritePin(AnalogPin.P0, 0)
})
basic.showIcon(IconNames.Happy)
```
# Explication du code
Le code que nous avons élaboré permet d'offrir 2 possibilités. Premièrement, lorsque nous allons appuyer sur le bouton A, le servo moteur tournera à 180 degrés.

En deuxième lieu, lorsque nous allons appuyer sur le bouton B, le servo moteur tournera dans le sens opposé.
