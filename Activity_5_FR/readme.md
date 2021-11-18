# Activité 5

# Partie 1 - Activité de programmation d’un micro:bit : Interconnexion des b.Boards
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

# Étape 2 : Signal radio
1. dans l'onglet ``||radio||`` recherchez le bloc ``||radio set group 1||`` dans le bloc ``||on start||``
2. dans l'onglet ``||Input||`` faites glisser le bloc ``||forever||`` et faites glisser le bloc ``||radio send string ""||`` et changez le **"" en bienvenue**
3. dans l'onglet ``||radio||``, faites glisser le ``||on radio receive receiveString||`` et faites glisser les blocs ``||show string "hello"||`` et remplacez le **"hello" par le ``||receivedString||``**
```
radio.onReceivedString(function (receivedString) {
    basic.showString(receivedString)
})
radio.setGroup(1)
basic.forever(function () {
    basic.showString("Welcome")
})
```
