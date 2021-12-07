# Activité 2

# Partie 1 - Activité de programmation d’un micro:bit : Faire allumer une lumière BliXel

Le micro:bit est un microcontrôleur simple et vous aurez la chance de faire des activités de codage qui vous permettront de mieux comprendre comment se protéger et du fonctionnement du monde de la cybersécurité. Nous vous accompagnerons avec ceci et vous pourrez aussi donner du temps aux élèves pour explorer et essayer de créer leurs propres programmes.
# Étape 1 : Branchez le câble USB du Microbit dans votre port USB

<!-- https://github.com/Brilliant-Labs/bboard-tuts-cybersecurity-3/blob/master/cybersec/activity-1/connect-microbit.gif?raw=true -->
![Click](https://github.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/blob/main/Activity_1/connect-microbit.gif?raw=true "Click")

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png -->
![click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_1/micro.png)

# Étape 2 : connectez le microbit au bboard et assurez-vous que l'alimentation est connectée

<!--https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/bborad.png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/b.Board_power.JPG)

# Etape 3 : Quand ton Microbit et brance 
1.trouvez l'onglet ``||BLixels:Blixels||`` une fois dans les ``||BLiXels:BLiXels||`` onglet cliquez et faites glisser ``||BLixels:set all blixels to red||`` et faites-le glisser dans le bloc pour toujours
2. allumez le bboard avec l'interrupteur sur le côté et voyez si le voyant est rouge
> (si les Blixels ne sont pas rouges) répétez l'étape 3 une fois de plus
<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(1).png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(1).png)

<!-- https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(2).png -->
![Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-cybersecurity-v3/main/Activity_2/image%20(2).png)

# Etape 4 : si le voyant est rouge
1. sous l'onglet ``||Variables:Variables||`` créez une toute nouvelle variable appelée **mot de passe**
2. une fois que vous avez défini votre nouvelle variable a été créée, faites glisser le ``||Variables:set password as 0||`` dans le bloc ``||basic:on start||`` également cliquez et faites glisser depuis le ``||basic:Basic||`` le ``||sbasic:how icon||`` et le changer du **coeur à oui** (1ère rangée, 3ème)
3. ``||Variables:set password to 0||`` bloquer et le changer en ``||Variables:set password to 123456||``

# Etape 5 : si tout fonctionne
1. à partir de l'onglet ``||Logic:Logic||`` faites glisser le bloc ``||Logic:if true then||`` et appuyez sur le bouton plus il devrait maintenant ressembler à ``||Logic:if true then else||``
2. saisir le  ``||BLiXles:set all Blixels to red||`` et le mettre dans le ``||Logic:if true then||`` et mettre un dans le ``||Logic:else||`` et changer celui dans le ``||Logic:if true then||`` à la couleur **vert** (2ème rangée, 1ère)
```blocks
let password = "123456"
basic.showIcon(IconNames.Yes)
basic.forever(function () {
    if (password == "123456") {
        BLiXel.showColour(0x00ff00)
    } else {
        BLiXel.showColour(0xff0000)
    }
))
```

# Explication du code
Nous avons commencé par créer une variable nommée password et nous l’avons placée dans le bloc au démarrage en lui assignant la valeur 123456. Ceci indique au micro:bit de créer la variable et d’y assigner le texte 123456 dès le démarrage du micro:bit.

Par la suite, nous avons inséré une petite logique dans le bloc toujours afin de spécifier au micro:bit ce qui se passerait dans le cas où notre variable n’aurait pas la même valeur que le mot de passe assigné à notre logique. Si le mot de passe de notre variable password (qui est créée au démarrage) est égal au texte 123456, alors, les lumières s’allument vertes. Sinon, les lumières s’allument rouges. Essayez de modifier le mot de passe à un endroit et voyez ce qui se passera.
