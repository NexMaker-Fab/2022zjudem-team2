<!-- project/presentation.md -->
# SOLAR PANEL TRACKING ENERGY

<br>
Our final goal is to build a self solar tracking energy and the vision is to capture as much as possible sunlight as a source of radiant energy, which is converted into electric energy in the form of direct current electricity. The project is based on LDR sensor, we made the rotatable Solar system which has the home position during night time but when the light is available in day time the solar system automatically waking up through sensing the light presence and all the solar panels rotate counter clockwise and open like a sunflower and follow the sun rotation, after the sun fallen down all the solar panels are automatically rotate clockwise and go to the home position for next day sun light.
<br>
<br>
Our Solar Panel tracking energy is a technology for orienting a solar collector, reflector, or photovoltaic panel towards the sun. As the sun moves across the sky, a tracking device makes sure that the solar collector automatically follows and maintains the optimum angle to receive the most of the solar radiation

<h1 style="font-size:1.5vw"><span style="color:black">I. Required Materials</span></h1>

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
<h1 style="font-size:1.5vw"><span style="color:black">II. Software Used</span></h1>

<a href="https://www.arduino.cc/en/software" class="fab fa-facebook"><span style="font-size:1.2vw">Arduino IDE</span></a>
<br>
<br><a href="https://easyeda.com/" class="fab fa-facebook"><span style="font-size:1.2vw">EasyEDA</span></a>
<br><br><a href="https://www.autodesk.com/products/fusion-360/free-trial" class="fab fa-facebook"><span style="font-size:1.2vw">Fusion 360</span></a>

<br>
<h1 style="font-size:1.5vw"><span style="color:black">III. Fusion 360 parts</span></h1>

<br>

<img src="images/fusion.jpg" alt="fusion.jpg" max-width="1200" height="800">

<br>
<h1 style="font-size:1.5vw"><span style="color:black">IV. How to make </span></h1>

<br>
We first bought the materials and printed the 3D parts 
<br>

<img src="images/allparts.jpg" alt="allparts.jpg" max-width="1200" height="800">

<br>After we used Easyeda to design the schematic and made our self custom pcb
<br><div class="loader"><img src="images/pcb.png" alt="#" /></div>
<br><div class="loader"><img src="images/pcb1.jpg" alt="#" /></div>

<br><br>
Now before we can try out the self custom pcb, we compiled and upload the codes to the arduino nano. The codes for this project can be found here.

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

After, we created a gerber file and orderd a custom pcb from [NEXTPCB](https://passport.hqonline.com/register?reurl=https%3A%2F%2Fwww.nextpcb.com%2Fregister%3Fcode%3Dtechboysxwd)

<br><div class="loader"><img src="images/nextpcb.jpg" alt="#" /></div>
<br><div class="loader"><img src="images/pcbf.jpg" alt="#" /></div>

<br>
<h1 style="font-size:1.5vw"><span style="color:black">Solar Panels connection </span></h1>
<br><div class="loader"><img src="images/solar panel.jpg" alt="#" /></div>
<br> 
<br> We are going to use 6 pieces of solar panel and each has 6V 70mAh power output, We will wire the one pair of panels in series and 3 pairs in parallel, then the voltage output will be 6+6=12v, So basically when the panels are fully opened the voltage output is 12V and when the panel goes on in home position the voltage output will be 1-3 volts.
<br><div class="loader"><img src="images/solars.jpg" alt="#" /></div>
<br><div class="loader"><img src="images/solarm.jpg" alt="#" /></div>
<br><div class="loader"><img src="images/solaro.jpg" alt="#" /></div>
<br>
<br> 
<h1 style="font-size:1.2vw"><span style="color:black">LDRS and Working Principle </span></h1>
<br>Light depending resistor is a photo-resistor, which decrease the resistance when the light increases.
An LDR or photo-resistor is made any semiconductor material with a high resistance. It has a high resistance because there are very few electrons that are free and able to move – the vast majority of the electrons are locked into the crystal lattice and unable to move. Therefore in this state there is a high LDR resistance.
<br>As light falls on the semiconductor, the light photons are absorbed by the semiconductor lattice and some of their energy is transferred to the electrons. This gives some of them sufficient energy to break free from the crystal lattice so that they can then conduct electricity. This results in a lowering of the resistance of the semiconductor and hence the overall LDR resistance.The process is progressive, and as more light shines on the LDR semiconductor, so more electrons are released to conduct electricity and the resistance falls further.
<br><div class="loader"><img src="images/solarl.jpg" alt="#" /></div>
<br>You can see the fifth resistor is placed on the middle position of the solar top,
when the light is minimum, the micro controller Arduino read the resistance value and the the threshold value is sated in the coding section, when the light is available and the threshold level breaks, the Arduino rotate the n20 gear motor anticlockwise through the L293D Driver till the limit switch level high, when anticlockwise limit switch pressed the panel stop rotating and panel is fully opened position when the button is pressed, now the main work is going to progress, according the sun rotation other 4 LDRs sense the light and send data to the Arduino, and Arduino process the data then rotate the servo motors according the sun rotation, the rotation position of the servo is max 170 degrees,when the sun goes down the fifth LDR sense data again and this time the process is reverse condition, the LDR data goes down blow the threshold level and Arduino Rotate the N20 motor clockwise till the 2nd limit switch press and run the servo in home position, when light is available in next day the same process goes on again.
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Project Circuit</span></h1>  
<br><div class="loader"><img src="images/solara.jpg" alt="#" /></div>



<br>
<h1 style="font-size:1.5vw"><span style="color:black">Innovation</span></h1>
Our Solar Panel Tracking Energy have 6 panels rotating at a 90-degree angle, producing 40% more energy than fixed solar panels. They work with a dual-axis tracking system, so they always face the sun — increasing productivity by up to 10%. Their elevated design also allows the panels to cool naturally, increasing their efficiency.

<br>
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Solar Flower Market- Global Industry Analysis and Forecast (2022-2029)</span></h1>
<br>The Global Solar Flower Market was valued at US $14 million in 2022 and is predicted to reach 39.20 million in 2028, at a compound annual growth rate of ( CAGR )16.00% between 2023 and 2028.

<br>Main benefits: Solar flower is a ground-mounted, all-in-one solar system with a tracker that follows the sun. It utilizes advanced automation to quickly monitor the sun, manufacturing up to 40% additional power than conventional static solar panels.
<br>Along with this, the solar flower possesses a unique feature of self-cleansing. Increase in recognition about the utilization of solar power and increase in advantages towards encouragement of sustainable power are major elements operating the global solar flower market. 
<br>Cons:However, the high initial investment and lack of skill professionals are the major factors restraining the global solar flower market.
<br>
<h1 style="font-size:1vw"><span style="color:black">Top Impacting Factors</span></h1>
Execution of strict rules to assist environmental preservation increases the energy industry to move to clean environment-friendly power resources. Moreover, the prices of power created using solar power is expected to decrease in the coming years, due to technological advancements.

<br>
<h1 style="font-size:1vw"><span style="color:black">Market Trends</span></h1>
● Awareness towards Environment and Use of Renewable Resources for Energy Generation Process
<br>● With increase in awareness about the carbon emission from several non-renewable resources and the rise in prices of fuels, the solar flower market is expected to have a surge in demand.
<br>● Favorable Government Policies and Priority is Key Driver for Market Growth
<br>● Technological Advancements and Increase in R&D Programs in Solar Energy Field is a Positive Factor for Growth of Market
<br>● Increase in demand for eco-friendly sources of energy coupled with advancement in the field of solar power generation technique had a positive impact on the market of solar flower.

<br>
<h1 style="font-size:1vw"><span style="color:black">Solar Flower Market Segment Analysis:</span></h1>

<br>Solar Flower Market is divided by: 
<br>Connectivity (On Grid and Off Grid)
<br>The off-grid segment is expected to enlarge at a quicker CAGR throughout the projected period.
<br>Application (Residential area, Schools and Universities, Recreational Parks, Mountainous Region, and Others)
<br>The schools and universities segment are estimated to enlarge at a quicker rate, due to the enormous scale implementations of solar flowers located in Europe and the U.S. 
<br>Region (North America, Europe, Asia Pacific, Middle East and Africa, and Latin America)
<br>North America is estimated to be the dominant region in the solar flower market. Development in expenditure in solar implementations is the major factor estimated to increase the market in the zone in the coming year. The U.S influenced the solar flower market in North America in 2021. 
<br>In July 2021, Virginia Wesleyan University became one of the first institutes in the nation to implement the smart flower, an advanced kind of solar function. The Asia Pacific is an alternate major zone of the worldwide solar flower market.
