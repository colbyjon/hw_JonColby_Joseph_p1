float r = 0;
float a = 0;
float backR;
float backG;
float backB;

void setup() {
  size(600, 600);
  backR = random(0, 100);
  backG = random(0, 100);
  backB = random(0, 100);
  
  background(0);
  rectMode(CENTER);
  
  noStroke();
  smooth();
}

void draw() 
{
  fill(backR, backG, backB, 50);
  rect(width/2, height/2, width, height);
  
    fill(255);
   translate(mouseX,mouseY);
   rotate(a);
    rect(0,0,100,100);
    
     fill(255);
   resetMatrix();
   translate(100,100);
   rotate(r);
    rect(0,0,5,50);
  
    fill(255);
   resetMatrix();
   translate(200,200);
   rotate(r);
    rect(0,0,150,50);
    
      fill(255);
   resetMatrix();
   translate(300,300);
   rotate(r);
    rect(0,0,400,50);
    
      fill(255);
  resetMatrix();
   translate(400,100);
   rotate(r);
    rect(0,0,100,200);
  
  
  r = r + 0.02;
  a = a + 0.05;
}
