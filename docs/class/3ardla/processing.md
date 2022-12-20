<!-- Processing/processing.md -->
<h1 style="font-size:2vw"><span style="color:black">PROCESSING</span></h1>
<h1 style="font-size:1.5vw"><span style="color:black">Introduction</span></h1>
<br>

[Processing](https://processing.org/download) is a flexible software sketchbook and a language for learning how to code within the context of the visual arts. Since 2001, Processing has promoted software literacy within the visual arts and visual literacy within technology. There are tens of thousands of students, artists, designers, researchers, and hobbyists who use Processing for learning and prototyping.
<br>Processing is a free graphical library and integrated development environment (IDE) built for the electronic arts, new media art, and visual design communities with the purpose of teaching non-programmers the fundamentals of computer programming in a visual context.

<br>Processing uses the Java language, with additional simplifications such as additional classes and aliased mathematical functions and operations. It also provides a graphical user interface for simplifying the compilation and execution stage.

<br>The Processing language and IDE have been the precursor to other projects including Arduino and Wiring.

- [Download Software](https://processing.org/download)

<h1 style="font-size:1.5vw"><span style="color:black">Similar Softwares</span></h1>

[Processing.js](https://www.tutorialspoint.com/online_processingjs_editor.php)
<br>Processing.js is an open programming language, port of the processing Visualization Language, for people who want to program images, animation, and interactions for the web without using Flash or Java applets. Processing.
<br>

[Vvvv](https://www.visualprogramming.net/)
<br>vvvv is a graphical programming environment for easy prototyping and development. It is designed to facilitate the handling of large media environments with physical interfaces, real-time motion graphics, audio and video that can interact with many users simultaneously.
<br>

[OpenFrameworks](https://openframeworks.cc/download/)
<br>openFrameworks is an open source C++ toolkit designed to assist the creative process by providing a simple and intuitive framework for experimentation.

<h1 style="font-size:1.2vw"><span style="color:black">Reference</span></h1>

- [Nexmaker](https://www.nexmaker.com/doc/10Interface-application-programming/processing.html)
- [Learning Processing](https://www.amazon.com/gp/product/0123944430/ref=as_li_ss_tl?ref_=nav_ya_signin&linkCode=sl1&tag=processing09-20&linkId=fb0eeedd8fb1016a790e83d538a1c030)


<h1 style="font-size:1.5vw"><span style="color:black">Processing Demo</span></h1>
<h1 style="font-size:1vw"><span style="color:black">Mouse Interaction</span>: Reach</h1>

The arm follows the position of the mouse by calculating the angles with [atan2()](https://processing.org/reference/atan2_.html).
<div class="loader"><img src="images/mouse.gif" alt="mouse.gif"max-width="800" height="500" />

<h1 style="font-size:1vw"><span style="color:black">Codes</span></h1>


```html
/**
 * Reach 2  
 * based on code from Keith Peters.
 * 
 * The arm follows the position of the mouse by
 * calculating the angles with atan2(). 
 */

int numSegments = 10;
float[] x = new float[numSegments];
float[] y = new float[numSegments];
float[] angle = new float[numSegments];
float segLength = 26;
float targetX, targetY;

void setup() {
  size(640, 360);
  strokeWeight(20.0);
  stroke(255, 100);
  x[x.length-1] = width/2;     // Set base x-coordinate
  y[x.length-1] = height;  // Set base y-coordinate
}

void draw() {
  background(0);
  
  reachSegment(0, mouseX, mouseY);
  for(int i=1; i<numSegments; i++) {
    reachSegment(i, targetX, targetY);
  }
  for(int i=x.length-1; i>=1; i--) {
    positionSegment(i, i-1);  
  } 
  for(int i=0; i<x.length; i++) {
    segment(x[i], y[i], angle[i], (i+1)*2); 
  }
}

void positionSegment(int a, int b) {
  x[b] = x[a] + cos(angle[a]) * segLength;
  y[b] = y[a] + sin(angle[a]) * segLength; 
}

void reachSegment(int i, float xin, float yin) {
  float dx = xin - x[i];
  float dy = yin - y[i];
  angle[i] = atan2(dy, dx);  
  targetX = xin - cos(angle[i]) * segLength;
  targetY = yin - sin(angle[i]) * segLength;
}

void segment(float x, float y, float a, float sw) {
  strokeWeight(sw);
  pushMatrix();
  translate(x, y);
  rotate(a);
  line(0, 0, segLength, 0);
  popMatrix();
}
```

- [Reference](https://processing.org/examples/reach2.html)

<h1 style="font-size:1vw"><span style="color:black">Keyboard Interaction</span>: Snake game</h1>
This is a simple snake game and a test for creating small games in processing
<div class="loader"><img src="images/snakegame.gif" alt="snakegame.gif"max-width="800" height="500" />
<h1 style="font-size:1vw"><span style="color:black">Codes</span></h1>

```html


//BY Ian151 (ChromeWing)
//inspired by the original snake game
//this is a test for creating small games in processing.

int angle=0;
int snakesize=5;
int time=0;
int[] headx= new int[2500];
int[] heady= new int[2500];
int applex=(round(random(47))+1)*8;
int appley=(round(random(47))+1)*8;
boolean redo=true;
boolean stopgame=false;
void setup()
{
  restart();
  size(400,400);
  textAlign(CENTER);
}
void draw()
{
  if (stopgame)
  {
    //do nothing because of game over (stop playing)
  }
  else
  {
    //draw stationary stuff
  time+=1;
  fill(255,0,0);
  stroke(0);
  rect(applex,appley,8,8);
  fill(0);
  stroke(0);
  rect(0,0,width,8);
  rect(0,height-8,width,8);
  rect(0,0,8,height);
  rect(width-8,0,8,height);
  //my modulating time by 5, we create artificial frames each 5 frames
  //(otherwise the game would go WAY too fast!)
  if ((time % 5)==0)
  {
    travel();
    display();
    checkdead();
  }
  }
}
//controls:
void keyPressed()
{
  if (key == CODED)
  {
    //what key was pressed? is the previous angle the opposite direction?
    //we wouldn't want to go backwards into our body, that would hurt!
    //also, is the previous body segment in front of the direction? 
    //(based on the previous question, but added for secure turning without suicide)
    if (keyCode == UP && angle!=270 && (heady[1]-8)!=heady[2])
    {
      angle=90;
    }
    if (keyCode == DOWN && angle!=90 && (heady[1]+8)!=heady[2])
    {
      angle=270;
    }if (keyCode == LEFT && angle!=0 && (headx[1]-8)!=headx[2])
    {
      angle=180;
    }if (keyCode == RIGHT && angle!=180 && (headx[1]+8)!=headx[2])
    {
      angle=0;
    }
    if (keyCode == SHIFT)
    {
      //restart the game by pressing shift
      restart();
    }
  }
}
void travel()
{
  for(int i=snakesize;i>0;i--)
  {
    if (i!=1)
    {
      //shift all the coordinates back one array
      headx[i]=headx[i-1];
      heady[i]=heady[i-1];
    }
    else
    {
      //move the new spot for the head of the snake, which is
      //always at headx[1] and heady[1].
      switch(angle)
      {
        case 0:
        headx[1]+=8;
        break;
        case 90:
        heady[1]-=8;
        break;
        case 180:
        headx[1]-=8;
        break;
        case 270:
        heady[1]+=8;
        break;
      }
    }
  }
  
}
void display()
{
  //is the head of the snake eating the apple?
  if (headx[1]==applex && heady[1]==appley)
  {
    //grow and spawn the apple somewhere away from the snake
    //(currently some of the code below might not be working, but the game still works.)
    snakesize+=round(random(3)+1);
    redo=true;
    while(redo)
    {
      applex=(round(random(47))+1)*8;
      appley=(round(random(47))+1)*8;
      for(int i=1;i<snakesize;i++)
      {
        
        if (applex==headx[i] && appley==heady[i])
        {
          redo=true;
        }
        else
        {
          redo=false;
          i=1000;
        }
      }
    }
  }
  //draw the new head of the snake...
  stroke(sinecolor(1),sinecolor(0),sinecolor(.5));
  fill(0);
  rect(headx[1],heady[1],8,8);
  //...then erase the back end of the snake.
  fill(255);
  rect(headx[snakesize],heady[snakesize],8,8);
  
}
void checkdead()
{
  for(int i=2;i<=snakesize;i++)
  {
    //is the head of the snake occupying the same spot as any of the snake chunks?
    if (headx[1]==headx[i] && heady[1]==heady[i])
    {
      fill(255);
      rect(125,125,160,100);
      fill(0);
      text("GAME OVER",200,150);
      text("Score:  "+str(snakesize-1)+" units long",200,175);
      text("To restart, press Shift.",200,200);
      stopgame=true;
    }
    //is the head of the snake hitting the walls?
    if (headx[1]>=(width-8) || heady[1]>=(height-8) || headx[1]<=0 || heady[1]<=0)
    {
      fill(255);
      rect(125,125,160,100);
      fill(0);
      text("GAME OVER",200,150);
      text("Score:  "+str(snakesize-1)+" units long",200,175);
      text("To restart, press Shift.",200,200);
      stopgame=true;
    }
  }
}
void restart()
{
  //by pressing shift, all of the main variables reset to their defaults.
  background(255);
  headx[1]=200;
  heady[1]=200;
  for(int i=2;i<1000;i++)
  {
    headx[i]=0;
    heady[i]=0;
  }
  stopgame=false;
  applex=(round(random(47))+1)*8;
  appley=(round(random(47))+1)*8;
  snakesize=5;
  time=0;
  angle=0;
  redo=true;
}
float sinecolor(float percent)
{
  float slime=(sin(radians((((time +(255*percent)) % 255)/255)*360)))*255;
  return slime;
}

```

- [Reference](https://openprocessing.org/sketch/50988/#)