# Speed-Direction-Velocity2

float posicion_en_x = 1;
float velocidad_x = 5;
int direccion_x = 2;

float posicion_en_y = 1;
float velocidad_y= 3;
int direccion_y= 2;


void setup(){
  size(500,500);
}


void draw(){
  background(0);
  
    posicion_en_x = posicion_en_x + (velocidad_x *direccion_x);
    posicion_en_y = posicion_en_y + (velocidad_y *direccion_y);
 
   if(posicion_en_x > 400 || posicion_en_x < 0){
    
    direccion_x = direccion_x * -1;
    
}

if(posicion_en_y > 400  || posicion_en_y < 0){
  
  direccion_y = direccion_y * -1;
  
  }
  
  rect(posicion_en_x, posicion_en_y,100,100);
  
    }
