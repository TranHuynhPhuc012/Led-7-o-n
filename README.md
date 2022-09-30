int a=6,b=5,c=4,d=3,e=2,f=1,g=0;
void setup(){
pinMode(a,OUTPUT); pinMode(b,OUTPUT); pinMode(c,OUTPUT);
pinMode(d,OUTPUT);pinMode(e,OUTPUT);pinMode(f,OUTPUT);pinMode(g,OUTPUT);

}
void KHONG(){
digitalWrite(a,HIGH); digitalWrite(b,HIGH); digitalWrite(c,HIGH);
digitalWrite(d,HIGH); digitalWrite(e,HIGH); 
digitalWrite(f,HIGH); digitalWrite(g,LOW);
delay(1000);
}
void MOT(){
digitalWrite(a,LOW); digitalWrite(b,HIGH);
digitalWrite(c,HIGH);digitalWrite(d,LOW);
digitalWrite(e,LOW); digitalWrite(f,LOW);
digitalWrite(g,LOW); delay(1000);
}
void HAI(){
digitalWrite(a,HIGH); digitalWrite(b,HIGH); 
digitalWrite(c,LOW);digitalWrite(d,HIGH); 
digitalWrite(e,HIGH); digitalWrite(f,LOW);
digitalWrite(g,HIGH); delay(1000);
}
void BA(){
digitalWrite(a,HIGH);digitalWrite(b,HIGH);
digitalWrite(c,HIGH);digitalWrite(d,HIGH);
digitalWrite(e,LOW);digitalWrite(f,LOW);
digitalWrite(g,HIGH);delay(1000);
}
void BON(){
digitalWrite(a,LOW);digitalWrite(b,LOW);
digitalWrite(c,HIGH);digitalWrite(d,LOW);
digitalWrite(e,LOW);digitalWrite(f,HIGH);
digitalWrite(g,HIGH);delay(1000);
}
void NAM(){
for (int i = 6; i >= 0; i--)
{
if(i != 2 && i != 5) digitalWrite(i,HIGH);  
else  digitalWrite(i,LOW); 
} delay(1000);
}
void SAU(){
for (int i = 6; i >= 0; i--)
{
if(i != 5) digitalWrite(i,HIGH);  
else  digitalWrite(i,LOW); 
} delay(1000);
}
void BAY(){
 for (int i = 6; i >= 0; i--)
{
if(i < 4) digitalWrite(i,LOW);  
else  digitalWrite(i,HIGH); 
} delay(1000);
}
void TAM()
{
 for (int i = 6; i >= 0; i--)
 digitalWrite(i, HIGH); 
 delay(1000);
}
void CHIN()
{
 for (int i = 6; i >= 0; i--)
 if(i!=2) digitalWrite(i, HIGH); 
 else digitalWrite(i, LOW); 
 delay(1000);
}
  void loop(){
   KHONG();
   MOT(); HAI();
   BA(); BON();
   NAM(); SAU();
   BAY();TAM();
   CHIN();    
}
