//declaring global variables
int w = 16;
int h = 16;
int index = 0;
//setting up the canvas and lines
void setup() {
 size(640, 384);
 background(#0000ff);
 strokeWeight(3);
 stroke(224);
 smooth();
}
//function to output lines
void draw() {
  //declaring positions of the lines
 int x1 = w*index;
 int x2 = x1 + w;
 int y1 = h*23;
 int y2 = h*24;
 //if randomized number is less than 0.8 then yellow forward slash is made
 if (random(1) < 0.8) {
 stroke(255, 238, 0);
 line(x2, y1, x1, y2);
 //if not then a pink backwards slash is made
 } else {
   stroke(238, 0, 255);
 line(x1, y1, x2, y2);
 }
 index++;
 //resetting variables if the slashes reach the end of the canvas
 if (index == width/w) {
 PImage p = get(0, h, width, h*23);
 background(#0000ff);
 set(0, 0, p);
 index = 0;
 }
}
