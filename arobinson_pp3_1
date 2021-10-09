/* Place two circles (of different sizes) at the center of the screen at 
opposite ends and have them move toward each other at different 
velocities. Whenever their edges touch the screen or each other, they
change direction. */

PVector location;
PVector velocity;
PVector size;

void setup()  {
  size(1000, 600);
  location = new PVector(width/5, width - (width/8));
  velocity = new PVector(width/800, -width/300);
  size = new PVector(width/5, width/8);
}  
void draw()  {
    background(255);
    stroke(255);
    fill(#ACB1C6, 170);
    ellipse(location.x, height/2, size.x, size.x);
    ellipse(location.y, height/2, size.y, size.y);
    location.add(velocity);
    if ((location.x < size.x/2)  ||  (location.x > (location.y - 1.3 * size.y))) {
      velocity.x = velocity.x * -1;
      }
      if (location.x > (location.y - 1.3 * size.y))  {
        velocity.y = velocity.y * -1;
      } else if  ((location.x < (location.y - 1.3 * size.y))  &&  (location.y > width - size.y/2))  {
      velocity.y = velocity.y * -1;
    }
}
