int count =0;
int fstx,fsty=0;

int Secx,Secy =0;

int THx,THy =0;

int Foux,Fouy =0;

void setup(){
 size(500,500);
}
void mousePressed(){ 
  if ( count ==0 ) {  
     fstx=mouseX;
     fsty=mouseY;
     count++;
  }else if (count ==1){
    Secx=mouseX;
    Secy=fsty;
    count++; 
  }else if (count ==2){
    THx=mouseX;
    THy=mouseY;
    count++;
  } else if (count ==3){
    Foux=mouseX; 
    Fouy=THy;
    count++;
  }
}
void draw(){
  background(255);
  if ( count ==0)
  {
    circle(mouseX, mouseY, 10);
    
  }
  if ( count ==1)
  {
    rect( fstx, fsty, mouseX-fstx, mouseY-fsty);
    
  }
  if (count == 2){
   rect(fstx , fsty , Secx-fstx, Secy-fsty);
   fill(255,0,0);
   text( "area:"+ (Secx-fstx)* (Secy-fsty), fstx,fsty-10);
   
  }
  if (count >= 3){
   quad(fstx , fsty , Secx-fstx, Secy-fsty,THx-Secx,THy-Secy,Foux-THx,Fouy-THy);
   fill(255,0,0);
   text( "area:"+ ((Secx-fstx)+ (Foux-THx))*(THy-fsty)/2, fstx,fsty-10);
   
  }
  
  
}
