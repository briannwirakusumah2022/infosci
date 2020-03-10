# This is my journal

1. What did we do?
  During Info Sceince we were told to instruct Dr. Reuben how to create a jelly sandwhich. 
  Dr. Reuben posed as an operator, essentially he could follow basic instructutions. 
  This forced us to create instructions with incredible detail. 
2. What did you learn?
  We learned basic computational thinking. There are four steps to Computational thinking: 
      1 decomposition 
      2 pattern recognition 
      3 abstraction 
      4 algorithm design
  To successfully create a jelly sandwhich, we had to use these four steps. 
3. What questions do you have?
    Will we be learning html? 
    
# Circles 

void setup (){
  size (1000, 1000);
  background (255);
}

void draw (){
ellipse(100, 100, 50, 50);
ellipse(125, 200, 50, 50);
ellipse(150, 300, 50, 50);
ellipse(175, 400, 50, 50);
ellipse(225, 300, 50, 50);
ellipse(250, 200, 50, 50);
ellipse(300, 300, 50, 50);
ellipse(325, 400, 50, 50);
ellipse(375, 300, 50, 50);
ellipse(400, 200, 50, 50);
ellipse(425, 100, 50, 50);
}
  
  
# Circles and Lines

x = 0

def setup():
    size(1000, 1000)
    background(255)
    textAlign(CENTER)
    
def draw():
   print("")
    
def mouseClicked():
    x = mouseX
    y = mouseY
    r = random(10,100)
    myred = random(0,255)
    myred = random(0, 255)
    myblue = random(0,255)
    mygreen = random(0,255)
    fill(myred, mygreen, myblue)
    
    line(500, 500, mouseX, mouseY)
    circle(x, y, r)
    fill(255)
    text("m", x,y)
    
    print (x, y)
    
# Moving Dice

rolls = 0
red_1 = 0 
orange = 0
yellow = 0 
green_1 = 0
blue_1 = 0
purple = 0
pink = 0

def setup():
    size (1000, 1000)
    background (255) 
    strokeWeight(5)
    
def draw():
    global rolls, red_1, orange, yellow, green_1, blue_1, purple, pink
    background (255)
    n = random(0,6)
    stroke(0)
    rect(100, 100, 400, 400, 25)
    stroke(255, 0, 0) #red green, blue
                   
    if 0<=n<1:
        # number one
        circle(300, 300, 50)
        red_1 = red_1 - 1
    if 1<=n<2:
        # number two 
        circle(200, 200, 50) # top left 
        circle(400, 400, 50) # bottom right
        orange = orange - 1
        stroke(240, 0, 0) #red green, blue
    if 2<=n<3:
        # number three 
        circle(300, 300, 50)
        circle(200, 200, 50) # top left 
        circle(400, 400, 50) # bottom right
        stroke(230, 0, 0) #red green, blue
    if 3<=n<4: 
        # number four 
        circle(200, 200, 50) # top left 
        circle(400, 400, 50) # bottom right
        circle(400, 200, 50) # top right
        circle(200, 400, 50) # bottom left
        green_1 = green_1 - 1 
    if 4<=n<5:
        # number five 
        circle(300, 300, 50)
        circle(200, 200, 50) # top left 
        circle(200, 400, 50) # bottom left
        circle(400, 200, 50) # top right
        circle(400, 400, 50) # bottom right
        blue_1 = blue_1 - 1
    if 5<=n<6: 
        # number six
        circle(200, 200, 50) # top left 
        circle(200, 300, 50) # middle left 
        circle(200, 400, 50) # bottom left
        circle(400, 300, 50) # middle right
        circle(400, 400, 50) # bottom right
        circle(400, 200, 50) # top right
        purple = purple - 1
    if 6<=n<7:
        # number seven 
        circle(200, 200, 50) # top left 
        circle(200, 300, 50) # middle left 
        circle(200, 400, 50) # bottom left
        circle(300, 300, 50) # center 
        circle(400, 300, 50) # middle right
        circle(400, 400, 50) # bottom right
        circle(400, 200, 50) # top right
        pink = pink - 1
    rolls += 1
    fill(0)
    textSize(20)
    text("Rolls:", 400, 550)
    text(rolls, 460,550)
    fill(255, 0, 0)
    rect(700, 700, 10, red_1)
    text("1", 700, 720)
    delay(200)
    rect(600, 700, 10, orange)
    text("2", 600, 720)
    stroke(255, 0, 0) #red green, blue
    rect(500, 700, 10, yellow)
    text("3", 500, 720)
    stroke(240, 0, 0) #red green, blue
    rect(400, 700, 10, green_1)
    text("4", 400, 720)
    stroke(230, 0, 0) #red green, blue
    rect(300, 700, 10, blue_1)
    text("5", 300, 720)
    stroke(220, 0, 0) #red green, blue
    rect(200, 700, 10, purple)
    text("6", 200, 720)
    stroke(210, 0, 0) #red green, blue
    fill(255)  
    
 # Optical Illusion 
 
 def setup():
    size(500, 500)
    background(255)
    
def draw():
    fill(0) 
    ellipse(100, 100, 100, 100)
    fill(0)
    ellipse(400, 100, 100, 100)
    fill(0)
    ellipse(250, 400, 100, 100)
    fill(0)
    
    stroke(0)
    strokeWeight (10)
    fill (255)
    triangle(250, 50, 100, 300, 400, 300)
    
    stroke(255)
    fill (255)
    triangle(100, 100, 400, 100, 250, 400)
    
    
# Traffic Light 

void setup()
{
  pinMode(13, OUTPUT);
  pinMode(12, OUTPUT);
  pinMode(11, OUTPUT);
}

void loop()
{
  digitalWrite(13, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(13, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(12, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(12, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(11, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(11, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(10, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(10, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(10, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(10, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(11, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(11, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(12, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(12, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(13, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(13, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
}



    
   
    
