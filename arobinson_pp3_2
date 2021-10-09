//  A real life example of this form of motion would be throwing a ball into the air.
//  The ball would acceleration upward, as it gradually slows down unitl
//  eventually its velocity becomes negative. The ball would accelerate downward and
//  we wouldn't bother catching it. 

PVector location;
PVector velocity;
PVector acceleration;
float r = random(1, 3);

void setup()  {
  size(1000, 600);
  location = new PVector(width/2, height - (width/16));
  acceleration = new PVector(0, .50);
  velocity = new PVector(0, r);
}
void draw()  {
  background(255);
  stroke(255);
  fill(#ACB1C6,170);
  ellipse(location.x, location.y, width/8, width/8);
  acceleration.y = acceleration.y - .0156;
  velocity.add(acceleration);
  location.sub(velocity);
}
