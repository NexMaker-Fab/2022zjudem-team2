<!-- project/presentation.md -->
# PANNEAU SOLAIRE QUI SUIT L'ENERGY SOLAIRE

<br>
Notre objectif final est de construire une énergie de suivi solaire autonome et la vision est de capter autant que possible la lumière du soleil comme source d'énergie rayonnante, qui est convertie en énergie électrique sous forme d'électricité à courant continu. Le projet est basé sur le capteur LDR, nous avons créé le système solaire rotatif qui a la position d'origine pendant la nuit, mais lorsque la lumière est disponible pendant la journée, le système solaire se réveille automatiquement en détectant la présence de lumière et tous les panneaux solaires tournent dans le sens inverse des aiguilles d'une montre. et ouvrez-vous comme un tournesol et suivez la rotation du soleil, après que le soleil soit tombé, tous les panneaux solaires tournent automatiquement dans le sens des aiguilles d'une montre et vont à la position d'origine pour la lumière du soleil du lendemain.
<br>
<br>
Notre énergie de suivi de panneau solaire est une technologie permettant d'orienter un capteur solaire, un réflecteur ou un panneau photovoltaïque vers le soleil. Au fur et à mesure que le soleil se déplace dans le ciel, un dispositif de suivi s'assure que le capteur solaire suit automatiquement et maintient l'angle optimal pour recevoir le maximum de rayonnement solaire

<h1 style="font-size:1.5vw"><span style="color:black">I. Matériaux nécessaires</span></h1>

<link rel="stylesheet" href="css/bootstrap-grid.min.css"/>
<div class="demo">
        <div class="container">
            <div class="row text-center">
                <h1 class="white"></h1>
            </div>

<div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/solar.jpg">
                        <div class="team-content">
                            <h3 class="title">Solar Panels(6pcs,6v each)</h3>
                        </div>
                    </div>
                </div>

<div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/battery.jpg">
                        <div class="team-content">
                            <h3 class="title">12V Li ion Battery</h3>
                        </div>
                    </div>
                </div>

<div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/nano.jpg">
                        <div class="team-content">
                            <h3 class="title">Arduino nano v3</h3>
                        </div>
                    </div>
                </div>
                 <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/l293d.jpg">
                        <div class="team-content">
                            <h3 class="title">L293d ic driver + ic base</h3>
                         </div>
                     </div>
                 </div>

<div class="row">
                     <div class="col-md-4 col-sm-6">
                         <div class="our-team">
                                 <img src="images/regulator.jpg">
                             <div class="team-content">
                                 <h3 class="title">7806 regulator</h3>
                        </div>
                    </div>
                </div>


<div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/resistor.jpg">
                        <div class="team-content">
                            <h3 class="title">10k carbon film resistor</h3>
                        </div>
                    </div>
                </div>
                <div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/ldr.jpg">
                        <div class="team-content">
                            <h3 class="title">ldrs</h3>
                        </div>
                    </div>
                </div>
                <div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/servo.jpg">
                        <div class="team-content">
                            <h3 class="title">servo motor</h3>
                        </div>
                    </div>
                </div>
<div class="row">
                 <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/gear.jpg">
                        <div class="team-content">
                            <h3 class="title">n20 gear motor</h3>
                         </div>
                     </div>
                 </div>
                <div class="row">
                     <div class="col-md-4 col-sm-6">
                         <div class="our-team">
                                 <img src="images/header.jpg">
                             <div class="team-content">
                                 <h3 class="title">male & female headers</h3>
                        </div>
                    </div>
                </div>

<div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/pcb.jpg">
                        <div class="team-content">
                            <h3 class="title">printed circuit board (pcb)</h3>
                        </div>
                    </div>
                </div>

<div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                            <img src="images/switch.jpg">
                        <div class="team-content">
                            <h3 class="title">limit switches</h3>
                        </div>
                    </div>
                </div>
</div>

<br>
<h1 style="font-size:1.5vw"><span style="color:black">II. Logiciel utilisé</span></h1>

<a href="https://www.arduino.cc/en/software" class="fab fa-facebook"><span style="font-size:1.2vw">Arduino IDE</span></a>
<br>
<br><a href="https://easyeda.com/" class="fab fa-facebook"><span style="font-size:1.2vw">EasyEDA</span></a>
<br><br><a href="https://www.autodesk.com/products/fusion-360/free-trial" class="fab fa-facebook"><span style="font-size:1.2vw">Fusion 360</span></a>

<br>
<h1 style="font-size:1.5vw"><span style="color:black">III. Fusion 360 parties</span></h1>

<br>

<img src="images/fusion.jpg" alt="fusion.jpg" max-width="1200" height="800">

<br>
<h1 style="font-size:1.5vw"><span style="color:black">IV. Comment le réaliser </span></h1>

<br>
Nous avons d'abord acheté les matériaux et imprimé les pièces en 3D 
<br>

<img src="images/allparts.jpg" alt="allparts.jpg" max-width="1200" height="800">

<br>Après avoir utilisé Easyeda pour concevoir le schéma et créer notre circuit imprimé personnalisé
<br><div class="loader"><img src="images/pcb.png" alt="#" /></div>
<br><div class="loader"><img src="images/pcb1.jpg" alt="#" /></div>

<br><br>
Maintenant, avant de pouvoir essayer le circuit imprimé personnalisé, nous avons compilé et téléchargé les codes sur l'arduino nano. Les codes de ce projet se trouvent ici.

```html

#include <Servo.h> 

Servo horizontal; // horizontal servo
int servoh = 180; 
int servohLimitHigh = 175;
int servohLimitLow = 5;
// 65 degrees MAX

Servo vertical; // vertical servo
int servov = 0; 
int servovLimitHigh = 60;
int servovLimitLow = 0;

// LDR pin connections
// name = analogpin;
int ldrlt = A1; //LDR top left - BOTTOM LEFT <--- BDG
int ldrrt = A2; //LDR top rigt - BOTTOM RIGHT
int ldrld = A3; //LDR down left - TOP LEFT
int ldrrd = A4; //ldr down rigt - TOP RIGHT
int ldrmt = A5;

const int button1 = 9;
const int button2 = 10; 
const int motorA =  7;
const int motorB =  8;
int buttonStateA = 0; 
int buttonStateB = 0; 

  int pos = 0;
  int pos2 = 0;
  int oldvalue;
  int oldvalue2;
  

void setup(){
  
horizontal.attach(5);
vertical.attach(6);
horizontal.write(180);
vertical.write(0);
  pinMode(motorA, OUTPUT);
  pinMode(motorB, OUTPUT);
  pinMode(button1, INPUT);
  pinMode(button1, INPUT);
delay(2500);
}
void loop() {
  int ldrStatus = analogRead(ldrmt);
  if (ldrStatus >30) {
    buttonStateA = digitalRead(button1);
     if (buttonStateA == LOW) {
    
    digitalWrite(motorA, HIGH); //COUNTER clockwise
    digitalWrite(motorB, LOW);
  }else{digitalWrite(motorA, LOW);
    digitalWrite(motorB, LOW);
    }

int lt = analogRead(ldrlt); // top left
int rt = analogRead(ldrrt); // top right
int ld = analogRead(ldrld); // down left
int rd = analogRead(ldrrd); // down right
int dtime = 10; int tol = 90; // dtime=diffirence time, tol=toleransi
int avt = (lt + rt) / 2; // average value top
int avd = (ld + rd) / 2; // average value down
int avl = (lt + ld) / 2; // average value left
int avr = (rt + rd) / 2; // average value right
int dvert = avt - avd; // check the diffirence of up and down
int dhoriz = avl - avr;// check the diffirence og left and rigt

//if(lt>90){
//if(Switch_a==LOW){
 // digitalWrite(9==HIGH);
// digitalWrite(10==LOW);
 // delay(1000);
//}}

if (-1*tol > dvert || dvert > tol) 
 {
 if (avt > avd)
 {
 servov = ++servov;
 if (servov > servovLimitHigh)
 {servov = servovLimitHigh;}
 }
 else if (avt < avd)
 {servov= --servov;
 if (servov < servovLimitLow)
 { servov = servovLimitLow;}
 }
 vertical.write(servov);
 }
if (-1*tol > dhoriz || dhoriz > tol) // check if the diffirence is in the tolerance else change horizontal angle
 {
 if (avl > avr)
 {
 servoh = --servoh;
 if (servoh < servohLimitLow)
 {
 servoh = servohLimitLow;
 }
 }
 else if (avl < avr)
 {
 servoh = ++servoh;
 if (servoh > servohLimitHigh)
 {
 servoh = servohLimitHigh;
 }
 }
 else if (avl = avr)
 {
 delay(10);
 }
 horizontal.write(servoh);
 }
  
 delay(dtime);
  

  }

else{
  oldvalue = horizontal.read();
  oldvalue2 = vertical.read();
  
 for (pos = oldvalue; pos <= 180; pos += 1) { // goes from 0 degrees to 180 degrees
    // in steps of 1 degree
    horizontal.write(pos);
    delay(15);
 }
    for (pos2 = oldvalue2; pos2 <= 0; pos2 += 1) { // goes from 0 degrees to 180 degrees
    // in steps of 1 degree
    
vertical.write(pos2);           // tell servo to go to position in variable 'pos'
    delay(15);}
    buttonStateB = digitalRead(button2);
    if (buttonStateB == LOW) {
    
    digitalWrite(motorA, LOW); //clockwise
    digitalWrite(motorB, HIGH);
  }else{digitalWrite(motorA, LOW);
    digitalWrite(motorB, LOW);
    }}}
```

<br><div class="loader"><img src="images/pcb2.jpg" alt="#" /></div>
<br><br>

Après, nous avons créé un fichier gerber et commandé un pcb personnalisé à partir de [NEXTPCB](https://passport.hqonline.com/register?reurl=https%3A%2F%2Fwww.nextpcb.com%2Fregister%3Fcode%3Dtechboysxwd)

<br><div class="loader"><img src="images/nextpcb.jpg" alt="#" /></div>
<br><div class="loader"><img src="images/pcbf.jpg" alt="#" /></div>

<br>
<h1 style="font-size:1.5vw"><span style="color:black">Connexion des panneaux solaires </span></h1>
<br><div class="loader"><img src="images/solar panel.jpg" alt="#" /></div>
<br> 
<br> Nous allons utiliser 6 panneaux solaires et chacun a une puissance de sortie de 6 V 70 mAh, nous allons câbler une paire de panneaux en série et 3 paires en parallèle, puis la tension de sortie sera de 6 + 6 = 12 V, donc fondamentalement quand le les panneaux sont complètement ouverts, la tension de sortie est de 12 V et lorsque le panneau s'allume en position initiale, la tension de sortie sera de 1 à 3 volts.
<br><div class="loader"><img src="images/solars.jpg" alt="#" /></div>
<br><div class="loader"><img src="images/solarm.jpg" alt="#" /></div>
<br><div class="loader"><img src="images/solaro.jpg" alt="#" /></div>
<br>
<br> 
<h1 style="font-size:1.2vw"><span style="color:black">LDRS et principe de fonctionnement </span></h1>
<br>La résistance dépendant de la lumière est une photo-résistance, qui diminue la résistance lorsque la lumière augmente.
Une LDR ou photo-résistance est constituée de tout matériau semi-conducteur à haute résistance. Il a une résistance élevée car il y a très peu d'électrons libres et capables de se déplacer - la grande majorité des électrons sont enfermés dans le réseau cristallin et incapables de se déplacer. Par conséquent, dans cet état, il existe une résistance LDR élevée.
<br>Lorsque la lumière tombe sur le semi-conducteur, les photons lumineux sont absorbés par le réseau semi-conducteur et une partie de leur énergie est transférée aux électrons. Cela donne à certains d'entre eux suffisamment d'énergie pour se libérer du réseau cristallin afin qu'ils puissent ensuite conduire l'électricité. Cela se traduit par une baisse de la résistance du semi-conducteur et donc de la résistance LDR globale. Le processus est progressif et, à mesure que la lumière brille sur le semi-conducteur LDR, davantage d'électrons sont libérés pour conduire l'électricité et la résistance diminue davantage.
<br><div class="loader"><img src="images/solarl.jpg" alt="#" /></div>
<br>Vous pouvez voir que la cinquième résistance est placée sur la position médiane du toit solaire,
lorsque la lumière est minimale, le microcontrôleur Arduino lit la valeur de résistance et la valeur de seuil est satisfaite dans la section de codage, lorsque la lumière est disponible et que le niveau de seuil se brise, l'Arduino fait tourner le moteur à engrenages n20 dans le sens inverse des aiguilles d'une montre via le pilote L293D jusqu'à le niveau de l'interrupteur de fin de course est élevé, lorsque l'interrupteur de fin de course dans le sens inverse des aiguilles d'une montre est enfoncé, le panneau arrête de tourner et le panneau est complètement ouvert lorsque le bouton est enfoncé, maintenant le travail principal va progresser, en fonction de la rotation du soleil, les 4 autres LDR détectent la lumière et envoient des données à l'Arduino et l'Arduino traitent les données puis font pivoter les servomoteurs en fonction de la rotation du soleil, la position de rotation du servo est de 170 degrés maximum, lorsque le soleil se couche à nouveau les données de détection LDR cinquième et cette fois le processus est inverse condition, le Les données LDR baissent le niveau de seuil et Arduino Faites tourner le moteur N20 dans le sens des aiguilles d'une montre jusqu'à ce que le 2ème interrupteur de fin de course appuie et fasse tourner le servo en position de repos, lorsque la lumière est disponible le lendemain, le même processus se répète.
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Circuit du projet</span></h1>  
<br><div class="loader"><img src="images/solara.jpg" alt="#" /></div>

<br>
<h1 style="font-size:1.5vw"><span style="color:black">Trials</span></h1>  
<br><br>
<img src="images/trial1.gif" alt="trial1.gif" max-width="1000" height="700">
<br><br>
<img src="images/trial1.gif" alt="trial2.gif" max-width="1000" height="700">
<br><br>
<img src="images/trial1.gif" alt="trial3.gif" max-width="1000" height="700">
<br>
<br>
<br><h1 style="font-size:1.5vw"><span style="color:black">Conception finale avec affichage de la puissance et du courant (voltage=11.14v, current=445mA and the power=4.978W)</span></h1> 
<br><div class="loader"><img src="images/display.jpg" alt="#" /></div>
<br><br><div class="loader"><img src="images/displayp.jpg" alt="#" /></div>
<br><br><div class="loader"><img src="images/displaypo.jpg" alt="#" /></div>
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Demo</span></h1> 
<br><br>
<img src="images/demo.gif" alt="demo.gif" max-width="1000" height="700">

<br>
<h1 style="font-size:1.5vw"><span style="color:black">Innovation</span></h1>
Notre énergie de suivi de panneau solaire a 6 panneaux tournant à un angle de 90 degrés, produisant 40 % d'énergie en plus que les panneaux solaires fixes. Ils fonctionnent avec un système de suivi à deux axes, de sorte qu'ils font toujours face au soleil, ce qui augmente la productivité jusqu'à 10 %. Leur conception surélevée permet également aux panneaux de se refroidir naturellement, augmentant ainsi leur efficacité.

<br>
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Marché des fleurs solaires – Analyse et prévisions de l’industrie mondiale (2022-2029)</span></h1>
<br>Le marché mondial des fleurs solaires était évalué à 14 millions de dollars américains en 2022 et devrait atteindre 39,20 millions en 2028, à un taux de croissance annuel composé (TCAC) de 16,00 % entre 2023 et 2028.

<br>Principaux avantages : Solar Flower est un système solaire tout-en-un monté au sol avec un tracker qui suit le soleil. Il utilise une automatisation avancée pour surveiller rapidement le soleil, produisant jusqu'à 40 % de puissance supplémentaire par rapport aux panneaux solaires statiques conventionnels.
<br>Parallèlement à cela, la fleur solaire possède une caractéristique unique d'auto-nettoyage. L'augmentation de la reconnaissance de l'utilisation de l'énergie solaire et l'augmentation des avantages pour l'encouragement de l'énergie durable sont des éléments majeurs du marché mondial des fleurs solaires.
<br>Inconvénients : Cependant, l'investissement initial élevé et le manque de compétences professionnelles sont les principaux facteurs qui freinent le marché mondial des fleurs solaires.
<br>
<h1 style="font-size:1vw"><span style="color:black">Principaux facteurs d'impact</span></h1>
L'exécution de règles strictes pour aider à la préservation de l'environnement incite l'industrie de l'énergie à passer à des ressources énergétiques propres et respectueuses de l'environnement. De plus, les prix de l'électricité créée à partir de l'énergie solaire devraient baisser dans les années à venir, en raison des progrès technologiques.

<br>
<h1 style="font-size:1vw"><span style="color:black">Tendances du marché</span></h1>
● Sensibilisation à l'environnement et à l'utilisation des ressources renouvelables pour le processus de production d'énergie
<br>● Avec une prise de conscience accrue des émissions de carbone de plusieurs ressources non renouvelables et de la hausse des prix des carburants, le marché des fleurs solaires devrait connaître une forte augmentation de la demande.
<br>● Les politiques gouvernementales favorables et la priorité sont le principal moteur de la croissance du marché
<br>● Les progrès technologiques et l'augmentation des programmes de R&D dans le domaine de l'énergie solaire sont un facteur positif pour la croissance du marché
<br>● L'augmentation de la demande de sources d'énergie respectueuses de l'environnement associée aux progrès dans le domaine de la technique de production d'énergie solaire a eu un impact positif sur le marché de la fleur solaire.

<br>
<h1 style="font-size:1vw"><span style="color:black">Analyse du segment de marché des fleurs solaires:</span></h1>

<br>Le marché aux fleurs solaires est divisé en :
<br>Connectivité (sur réseau et hors réseau)
<br>Le segment hors réseau devrait s'agrandir à un TCAC plus rapide tout au long de la période projetée.
<br>Application (zone résidentielle, écoles et universités, parcs de loisirs, région montagneuse et autres)
<br>On estime que le segment des écoles et des universités s'agrandit à un rythme plus rapide, en raison des mises en œuvre à grande échelle de fleurs solaires situées en Europe et aux États-Unis.
<br>Région (Amérique du Nord, Europe, Asie-Pacifique, Moyen-Orient et Afrique et Amérique latine)
<br>On estime que l'Amérique du Nord est la région dominante sur le marché des fleurs solaires. L'évolution des dépenses dans les implémentations solaires est le principal facteur estimé pour augmenter le marché dans la zone au cours de l'année à venir. Les États-Unis ont influencé le marché des fleurs solaires en Amérique du Nord en 2021.
<br>En juillet 2021, la Virginia Wesleyan University est devenue l'un des premiers instituts du pays à mettre en œuvre la fleur intelligente, un type avancé de fonction solaire. L'Asie-Pacifique est une autre zone majeure du marché mondial des fleurs solaires.


<h1 style="font-size:1.5vw"><span style="color:black">Analyse technique clé</span></h1>
<h1 style="font-size:1vw"><span style="color:black">*01 Cellule photovoltaïque (Solar PV) </span></h1>
<br><div class="loader"><img src="images/solar-photovoltaic-pv.jpeg" alt="#" /></div>
<br>La production solaire photovoltaïque a augmenté d'un record de 179 TWh (+ 22 %) en 2021 pour dépasser 1000 TWh. Il a démontré la deuxième plus grande croissance de production absolue de toutes les technologies renouvelables en 2021, après l'éolien. Le solaire photovoltaïque devient l'option la moins coûteuse pour la nouvelle production d'électricité dans la majeure partie du monde, ce qui devrait stimuler les investissements dans les années à venir. Cependant, une croissance annuelle moyenne de la production de 25 % sur la période 2022-2030 est nécessaire pour suivre le scénario zéro émission nette d'ici 2050. Cela correspond à une multiplication par plus de trois du déploiement annuel des capacités jusqu'en 2030, nécessitant une ambition politique beaucoup plus grande et davantage d'efforts de la part des acteurs publics et privés, en particulier dans les domaines de l'intégration du réseau et de l'atténuation des défis politiques, réglementaires et financiers. C'est particulièrement le cas dans les pays émergents et en développement.

<br>
<h1 style="font-size:1vw"><span style="color:black">*02 Arduino Nano v3</span></h1>
<br><div class="loader"><img src="images/v3.webp" alt="#" /></div>
<br>L'Arduino Nano est une petite carte complète et compatible avec les planches à pain basée sur l'ATmega328 (Arduino Nano 3.x). Il a plus ou moins les mêmes fonctionnalités que l'Arduino Duemilanove, mais dans un package différent. Il ne manque qu'une prise d'alimentation CC et fonctionne avec un câble USB Mini-B au lieu d'un câble standard. L'Arduino Nano peut être alimenté via la connexion USB Mini-B, une alimentation externe non régulée 6-20V (broche 30) ou une alimentation externe régulée 5V (broche 27). La source d'alimentation est automatiquement sélectionnée sur la source de tension la plus élevée.
<br>Chacune des 14 broches numériques du Nano peut être utilisée comme entrée ou sortie, en utilisant les fonctions pinMode(), digitalWrite() et digitalRead(). Ils fonctionnent à 5 volts. Chaque broche peut fournir ou recevoir un maximum de 40 mA et possède une résistance pull-up interne (déconnectée par défaut) de 20-50 kOhms. De plus, certaines broches ont des fonctions spécialisées :
<br>

* Serial: 0 (RX) and 1 (TX). Used to receive (RX) and transmit (TX) TTL serial data. These pins are connected to the corresponding pins of the FTDI USB-to-TTL Serial chip.
* External Interrupts: 2 and 3. These pins can be configured to trigger an interrupt on a low value, a rising or falling edge, or a change in value. See the attachInterrupt() function for details.
* PWM: 3, 5, 6, 9, 10, and 11. Provide 8-bit PWM output with the analogWrite() function.
* SPI: 10 (SS), 11 (MOSI), 12 (MISO), 13 (SCK). These pins support SPI communication, which, although provided by the underlying hardware, is not currently included in the Arduino language.
* LED: 13. There is a built-in LED connected to digital pin 13. When the pin is HIGH value, the LED is on, when the pin is LOW, it's off.
<br>The Nano has 8 analog inputs, each of which provide 10 bits of resolution (i.e. 1024 different values). By default they measure from ground to 5 volts, though is it possible to change the upper end of their range using the analogReference() function. Analog pins 6 and 7 cannot be used as digital pins. Additionally, some pins have specialized functionality:
<br>
* I2C: A4 (SDA) and A5 (SCL). Support I2C (TWI) communication using the Wire library (documentation on the Wiring website).
<br>
There are a couple of other pins on the board:

* AREF. Reference voltage for the analog inputs. Used with analogReference().
* Reset. Bring this line LOW to reset the microcontroller. Typically used to add a reset button to shields which block the one on the board.

<h1 style="font-size:1vw"><span style="color:black">*03 L293D IC Driver</span></h1>
<br><div class="loader"><img src="images/L293D.webp" alt="#" /></div>
<br>The L293D is a dual-channel H-Bridge motor driver capable of driving a pair of DC motors or a single stepper motor. This means it can drive up to two motors individually it's also one of the cheapest and easiest way to control dc motors through arduino boards, which makes it ideal for building this project.

<br>The L293D is most often used to drive motors, but can also be used to drive any inductive load such as a relay solenoid or large switching power transistor.It is capable of driving four solenoids, four uni-directional DC motors, two bi-directional DC motors or one stepper motor.

<br>
<h1 style="font-size:1vw"><span style="color:black">*04 PCB</span></h1>
<br><div class="loader"><img src="images/npcb.jpg" alt="#" /></div>
<br>One of the key concepts in electrical and electronics is the printed circuit board(PCB). It allows component to connect to one another in a safe and controlled manner. It is a board that has lines and pads that connect various points together, it also allows signals and power to be routed between physical devices
<br>Electrical components may be fixed to conductive pads on the outer layers in the shape designed to accept the component's terminals, generally by means of soldering, to both electrically connect and mechanically fasten them to it.

<br>
<h1 style="font-size:1.5vw"><span style="color:black">Our Project and the UN Sustainable Delevelopment Goals (SDGs)</span></h1>
<br>
The UN adopted 17 Sustainable Development Goals to improve People's leaving condition in the world.
<br>The Sustainable Development Goals are a call for action by all countries – poor, rich and middle-income – to promote prosperity and a better quality life while protecting the planet. They recognize that ending poverty and other deprivations must go hand-in-hand with strategies that build economic growth and address a range of social needs including social protection, health, education, job opportunities and reduce inequality, while tackling climate change and environmental protection.



<br>Our Project (Solar Pannel, power supply system) is in accordance with some of the UN SDGs Goals. As we all know, electricity is an indispensable part of daily life, and the generation of electricity marks the further liberation of productivity. Power system refers to completing the generation, transformation, transmission and distribution of electric energy. With the rapid change of science and technology, power technology has made great progress, and humans have also entered the electrical information area. Only a reliable, safe and affordable power supply and distribution system can ensure the normal work and life environment. Information technology and other high and new technology are built on the basis of electricity application, electric energy occupies a very important position in modern industrial production and the society at large.

<br>Our project include three of the SDGs Goals:

* SDG Goal 7 Affordable and Clean Energy
* SDG Goal 11 Sustainable Cities and Communities
* SDG Goal 13 Climate Action

<br>The sustainable development goals (SDGs) proposed by the Open Working Group of the General Assembly of the United Nations recognize the importance of the natural environment and its resources to human well-being. As a whole, it is definitely a worthy charter for the twenty-first century, as it addresses the diverse challenges that we face as a global community. SDG 7—to “ensure access to affordable, reliable, sustainable and modern energy for all”—is a challenge confronting every country, that touches everyone. To understand the necessity of meeting this goal, and what is required to do so, we should unpack the statement of the goal itself. The four dimensions of SDG 7 are affordability, reliability, sustainability and modernity. These different dimensions are not mutually exclusive. They overlap, and in some cases even entail each other.

<br>Consider what it means to have access to affordable energy. The heterogeneity of energy use across the world is due largely to different natural resource endowments and purchasing power. For example, a country with large coal deposits will likely make wide use of this resource to industrialize its economy. The people living within this country will likely use it as the primary means of power generation.
<br>On the other hand, people living in places without ready stocks of fossil fuels may rely on more primitive methods of combustion, such as wood fibers or perhaps even animal dungs. Indeed, this is the condition that prevailed for the vast majority of humankind throughout its history, and continues to be the condition for many parts of the developing world. For instance, approximately 2.7 billion people (about 40 per cent of the world’s population) now rely on traditional biomass fuels for cooking. Such low-quality fuels can be a major source of indoor air pollution. Even with the expansion of energy accessibility and economic development, the annual death toll from indoor air pollution will still be over 1.5 million people—a higher rate than that from both malaria and tuberculosis.

<br>As globalization continues to bind the world in deeper networks of trade, countries can augment and diversify their energy endowments by import. However, if the development level of a country is low and the costs of energy—which are increasingly determined by global financial forces—are high, then people will lack access to energy no matter how large or diverse its country’s endowment. Thus, an essential condition of affordability is raising income levels (and hence purchasing power) and controlling the impacts that impersonal economic forces operating at global levels have on the costs that people face on an everyday basis.

<br>Affordability is meaningless, however, if energy provision is unreliable. In many parts of the developing world, energy sources are often scarce and their supply intermittent. Today, 20 per cent of the world’s population still lacks access to electricity, and a larger share suffers from persistent power failures.3 In 2012, the massive, nationwide blackout that struck India affected nearly 700 million people, paralyzing transportation and communication systems and causing an unknown number of fatalities. This disaster was caused not just by supply issues, but also by mismanagement and an underdeveloped energy infrastructure. Thus, basic economic activity depends on a steady supply, robust governance, and an efficient and stable distribution system. There are multiple socioeconomic dimensions of energy reliability.

<br>Electricity, automated transportation and information technology are essential to economic development. They are also basic features of modern society, and thus energy sources and systems that meet these needs reliably and affordably can be considered as “modern”. Population growth will continue in India, sub-Saharan Africa, and other parts of the developing world. Per capita economic consumption will also increase, creating much greater demand for the services described above, and consequently for access to modern energy. Over the next quarter century, about 90 per cent of the growth in energy demand will come from countries that are not members of the Organization for Economic Co-operation and Development (OECD), i.e., countries outside of the rich Western economies and Japan.5Meeting this rising wave of energy demand will be one of the paramount challenges of the twenty-first century, and is a reason why it occupies such a central place in the SDGs. It also brings us to the final dimension of SDG 7: sustainability.

<br>Energy should generate a consistent stream of power to meet basic human needs, maintain and improve social functioning, and advance living standards. It should also fulfill these functions as sustainably as possible—that is to say, the power generated by energy use should be much greater than the resulting waste and pollution. All sustainable energy must be modern, although not all forms of modern energy are sustainable. Coal is perhaps the most important case in point. Historically, coal has been indispensable to industrialization and the advancement of human well-being. If more of the world’s people enjoy previously unimaginable living standards today, it is in large part because of coal. Offsetting its many virtues—for instance, abundance, wide distribution, and ease of use—is a long list of serious problems, however. In an age of population growth and environmental decline, this list is still growing.

<br>Today, coal still provides about 40 per cent of the world’s electricity and nearly the same fraction of global carbon emissions. Coal is also inefficient, with a low mass-to-energy ratio, and creates enormous pollution. Thus, coal is neither sustainable at the global scale because of its contribution to anthropogenic climate change, nor at the local scale because it is a threat to public health and ecological conditions (in addition to the polluting by-products of combustion, the process of coal mining creates myriad environmental problems). Given the scale of the use of coal, and the emergence of a global economy powered largely by fossil fuels, what can be done?

<br>These are challenges that require a pragmatic, multi-faceted approach. Solutions need to be found at the global scale, where Governments and agencies must work together. International climate change agreements are the most visible fruits of such efforts. The SDGs have also helped set the tenor for cooperation and contributed to an emerging consensus on priorities. In terms of policies, the transfer of clean energy technologies to developing countries is an important example. Indeed, international climate change agreements—such as the clean development mechanism (CDM)—explicitly provide for such transfers. This is not enough, however. Solutions must also be developed locally. There is evidence that benefits from CDM, while necessary and net-positive generally, do not always reach the local level, particularly in impoverished rural areas. Development should be sensitive to local conditions, and identify unintended consequences of energy policies. The heedless pursuit of biofuels at the global and regional levels may result in unintended yet severe environmental degradation. The countless acres of land deforested for palm oil undermine local well-being, and provide a stark reminder of the complexity of the energy problems that we face.

<br>Access to affordable, reliable, sustainable and modern energy is integral to global development in the twenty-first century. Not all the solutions needed to meet this challenge are yet available, and those that are may not be apparent. Figuring out these solutions and aligning them across scales will be difficult. Yet the task is achievable if international organizations have sufficient vision, if Governments can work together, and if communities and individuals are offered the right incentives and the necessary means. SDG 7 is, at the very least, an important step in that direction.   

<br>INCLUSIVE, SAFE, RESILIENT AND SUSTAINABLE
<br>The 11th goal is to promote sustainable development on urban areas by making cities and human settlements inclusive, safe, resilient, and sustainable.
Currently many people leave the rural areas to find better opportunities in the urban areas increasing the population in the urban areas, although this growth can lead to a variety of problems, including financial, social and environmental inequalities 

<br>A sustainable city reduces environmental impacts through its activities and promotes sustainable consumption and production patterns in accordance with its own territorial, geographical, social, economic, and cultural conditions. It is a city that is resilient to the impacts of climate change reducing the vulnerabilities of its population. The perfect sustainable city would be one that is self-sufficient in energy, manages waste to produce energy, has more sustainable transport, maintains green spaces and manages and uses its natural resources correctly.

<br>A sustainable city requires a lot of eco-friendly planning including CITY-WIDE ACCESS TO PUBLIC TRANSPORTATION; PEDESTRIAN- AND BIKE-FRIENDLY SIDEWALKS; SUSTAINABLE ARCHITECTURE the use of renewable energy and so on. One of the biggest indicators of a sustainable city is their efforts to switch to clean energy. Consequently, the use of solar panels is necessary as it will be:

<br>Financially beneficial- lower electricity bill
Environmentally friendly- Each kilowatt-hour (kWh) of solar that is generated will substantially reduce greenhouse gas emissions like CO2, as well as other dangerous pollutants such as sulfur oxides, nitrogen oxides and particulate matter.  Solar also reduces water consumption and withdrawal.


<br>Take urgent action to combat climate change and its impacts.
Climate change refers to long-term shifts in temperatures and weather patterns. These shifts may be natural, such as through variations in the solar cycle. But since the 1800s, human activities have been the main driver of climate change, primarily due to burning fossil fuels like coal, oil and gas.

<br>Burning fossil fuels generates greenhouse gas emissions that act like a blanket wrapped around the Earth, trapping the sun’s heat and raising temperatures.

<br>Examples of greenhouse gas emissions that are causing climate change include carbon dioxide and methane. These come from using gasoline for driving a car or coal for heating a building, for example. Clearing land and forests can also release carbon dioxide. Landfills for garbage are a major source of methane emissions. Energy, industry, transport, buildings, agriculture and land use are among the main emitters.
<br>People are experiencing climate change in diverse ways.
<br>Climate change can affect our health, ability to grow food, housing, safety and work. Some of us are already more vulnerable to climate impacts, such as people living in small island nations and other developing countries. Conditions like sea-level rise and saltwater intrusion have advanced to the point where whole communities have had to relocate, and protracted droughts are putting people at risk of famine. In the future, the number of “climate refugees” is expected to rise.
<br>We face a huge challenge but already know many solutions.
<br>Switching energy systems from fossil fuels to renewables like solar or wind will reduce the emissions driving climate change.
<br>As a renewable source of power, solar energy has an important role in reducing greenhouse gas emissions and mitigating climate change, which is critical to protecting humans, wildlife, and ecosystems. Solar energy can also improve air quality and reduce water use from energy production.



<br>So the use of solar panel is necessary nowadays to mitigate the impacts caused by climate change.