int n1=12,n2=11,n3=10,n4=9, e1=5,e2=3; 
 char a;
 void setup() 
 {
 pinMode(n1,OUTPUT);
 pinMode(n2,OUTPUT);
 pinMode(n3,OUTPUT);
 pinMode(n4,OUTPUT);
 pinMode(e1,OUTPUT);
 pinMode(e2,OUTPUT);
 Serial.begin(9600);
 }
 void loop() 
 {
 if(Serial.available()>0)
 a = Serial.read();
 Serial.println(a);

 if(a=='F')
 {
 Serial.println("F");
 digitalWrite(n1,HIGH); //forward
 digitalWrite(n2,LOW);
 digitalWrite(n3,HIGH);
 digitalWrite(n4,LOW);
 analogWrite(e1,255);
 analogWrite(e2,255);
 }

 else if(a=='B')
 {
 Serial.println("B");
 digitalWrite(n1,LOW); //backward
 digitalWrite(n2,HIGH);
 digitalWrite(n3,LOW);
 digitalWrite(n4,HIGH);
 analogWrite(e1,155);
 analogWrite(e2,155);
 }


 else if(a=='R')
 {
 Serial.println("R");
 digitalWrite(n1,LOW); //right
 digitalWrite(n2,LOW);
 digitalWrite(n3,LOW);
 digitalWrite(n4,HIGH);
 analogWrite(e1,155);
 analogWrite(e2,155);
 }
 else if(a=='L')
 {
 Serial.println("L");
 digitalWrite(n1,HIGH); //left
 digitalWrite(n2,LOW);
 digitalWrite(n3,LOW);
 digitalWrite(n4,LOW);
 analogWrite(e1,155);
 analogWrite(e2,155);
 }
 else
 {
 Serial.println("Invalid");
 digitalWrite(n1,LOW); //stop
 digitalWrite(n2,LOW);
 digitalWrite(n3,LOW);
 digitalWrite(n4,LOW);
 analogWrite(e1,0);
 analogWrite(e2,0);
 }
}
