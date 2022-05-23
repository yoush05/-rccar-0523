# -rccar-0523

int motor1PinA  = 2 ;
int motor1PinB =3 ;
int enablelPin=  11 ; 
int motor2PinA  =4;
int motor3PinB =5;
int enableRpin =10;

  void setup() {
     pinMode(motor1PinB, OUTPUT);
     pinMode(enablelPin, OUTPUT);
     analogWrite(enablelPin,150);
     pinMode(motor3PinB, OUTPUT);
     pinMode(enableRpin, OUTPUT);
     analogWrite(enableRpin, 150);
  }
   void loop() {
     digitalWrite(motor1PinA, LOW);
     digitalWrite(motor1PinB, HIGH);
     digitalWrite(motor2PinA, LOW);
     digitalWrite(motor3PinB, HIGH);
     delay(1000);
     
     low와 high로 둘다 두는 이유는 회로를 이용하기 위해서이다. 

     digitalWrite(motor1PinA, HIGH);
     digitalWrite(motor1PinB, LOW);
     digitalWrite(motor2PinA, HIGH);
     digitalWrite(motor3PinB, LOW);
     delay(1000);

     digitalWrite(motor1PinA, HIGH);
     digitalWrite(motor1PinB, HIGH);
     digitalWrite(motor2PinA, LOW);
     digitalWrite(motor3PinB, HIGH);
     delay(1000);

     digitalWrite(motor1PinA, LOW);
     digitalWrite(motor1PinB, HIGH);
     digitalWrite(motor2PinA, LOW);
     digitalWrite(motor3PinB, LOW);
     delay(1000);

     
     }
    
