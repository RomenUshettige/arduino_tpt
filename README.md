# DADO
Quest'esperienza riguarda l'utilizzo di Arduino al fine di far tirare un dado elettrico che in base ai led che accende equivale al numero.

### MATERIALE UTILIZZATO
- Resistenza a 220 O
- Led (rosso)
- Collegamenti
- Kit Sparkfun

### CODICE ARDUINO
Per l'esperienza di DADO abbiamo utilizzato il seguente codice:
>const int pin_ledblu7=7;  
const int pin_ledblu6=6;  
const int pin_ledblu5=5;  
const int pin_ledblu4=4;    
const int pin_ledblu3=3;  
const int pin_ledblu2=2;  
const int pin_ledblu1=1;  
int X=0;  
  
>   void setup(){   
pinMode(pin_ledblu7,OUTPUT);  
pinMode(pin_ledblu6,OUTPUT);  
pinMode(pin_ledblu5,OUTPUT);  
pinMode(pin_ledblu4,OUTPUT);  
pinMode(pin_ledblu3,OUTPUT);   
pinMode(pin_ledblu2,OUTPUT);   
pinMode(pin_ledblu1,OUTPUT);  
}  
 
> void loop() {  
X=random(1,6);  
if( X==1){  
digitalWrite(pin_ledblu7,HIGH);   
  }  
if( X==2){  
digitalWrite(pin_ledblu1,HIGH);  
digitalWrite(pin_ledblu6,HIGH);  
  }  
if( X==3){  
digitalWrite(pin_ledblu1,HIGH);  
digitalWrite(pin_ledblu7,HIGH);  
digitalWrite(pin_ledblu6,HIGH);   
  }  
if( X==4){  
digitalWrite(pin_ledblu1,HIGH);   
digitalWrite(pin_ledblu4,HIGH);   
digitalWrite(pin_ledblu3,HIGH);  
digitalWrite(pin_ledblu6,HIGH);  
  }  
if( X==5){  
digitalWrite(pin_ledblu1,HIGH);  
digitalWrite(pin_ledblu4,HIGH);  
digitalWrite(pin_ledblu3,HIGH);  
digitalWrite(pin_ledblu6,HIGH);  
digitalWrite(pin_ledblu7,HIGH);  
  }  
if( X==6){  
digitalWrite(pin_ledblu1,HIGH);  
digitalWrite(pin_ledblu2,HIGH);  
digitalWrite(pin_ledblu3,HIGH);  
digitalWrite(pin_ledblu4,HIGH);  
digitalWrite(pin_ledblu5,HIGH);  
digitalWrite(pin_ledblu6,HIGH);  
}  
delay(5000);//attendi 5000 millisecondi  
  
>digitalWrite(pin_ledblu1,LOW);  
digitalWrite(pin_ledblu2,LOW);  
digitalWrite(pin_ledblu3,LOW);  
digitalWrite(pin_ledblu4,LOW);  
digitalWrite(pin_ledblu5,LOW);  
digitalWrite(pin_ledblu6,LOW);  
digitalWrite(pin_ledblu7,LOW);  
delay(3000);//attendi 3000 millisecondi  

>} 

### CONCLUSIONI
Dopo aver eseguito il programma, come da codice, il led inizia a eseguire il 
comando di accensione e spegnimento entrando nel loop e svolge tutto all'infinito 
fino a che non si stoppa.

**AUTHOR**
Coppini Rudy
