#include <SoftwareSerial.h>

SoftwareSerial BT(9, 10);

#define AIN1 4
#define AIN2 5
#define PWMA 3

#define BIN1 8
#define BIN2 7
#define PWMB 6

float val;
float speed = 0;
char ch;
void setup() {
  
  pinMode(AIN1, OUTPUT);
  pinMode(AIN2, OUTPUT);
  pinMode(PWMA, OUTPUT);

  pinMode(BIN2, OUTPUT);
  pinMode(BIN1, OUTPUT);
  pinMode(PWMB, OUTPUT);

  Serial.begin(9600);
  BT.begin(9600);


  digitalWrite(AIN1, HIGH);
  digitalWrite(AIN2, LOW);
  digitalWrite(BIN1, HIGH);
  digitalWrite(BIN2, LOW);

}

void loop() {
  
  //PC to Phone
  if (BT.available()) {
    
    ch = BT.read();

    Serial.write(ch);
    
    if(ch >= '0' && ch <= '9'){
    val = ch - '0';
    speed = map(val, 0, 9, 0, 255);
    }

  
  switch (ch) {
        
        case 'F':
          digitalWrite(AIN1, LOW);
          digitalWrite(AIN2, HIGH);

          digitalWrite(BIN1, LOW);
          digitalWrite(BIN2, HIGH);

          analogWrite(PWMA, speed);
          analogWrite(PWMB, speed);
          Serial.println(" Forward");
          break;
        
        case 'B': 
          digitalWrite(AIN1, HIGH);
          digitalWrite(AIN2, LOW);

          digitalWrite(BIN1, HIGH);
          digitalWrite(BIN2, LOW);

          analogWrite(PWMA, speed);
          analogWrite(PWMB, speed);
          Serial.println(" Backward");
          break;

        case 'R':
          digitalWrite(AIN1, HIGH);
          digitalWrite(AIN2, LOW);

          digitalWrite(BIN1, LOW);
          digitalWrite(BIN2, HIGH);

          analogWrite(PWMA, speed);
          analogWrite(PWMB, speed);
          Serial.println(" LEFT");
          break;

        case 'L':
          digitalWrite(AIN1, LOW);
          digitalWrite(AIN2, HIGH);

          digitalWrite(BIN1, HIGH);
          digitalWrite(BIN2, LOW);

          analogWrite(PWMA, speed);
          analogWrite(PWMB, speed);
          Serial.println(" LEFT");
          break;
          
          case 'G':
          digitalWrite(AIN1, LOW);
          digitalWrite(AIN2, HIGH);

          digitalWrite(BIN1, LOW);
          digitalWrite(BIN2, HIGH);

          analogWrite(PWMA, speed);
          analogWrite(PWMB, speed/2);
          Serial.println(" FORWARD-LEFT");
          break;

          case 'I':
          digitalWrite(AIN1, LOW);
          digitalWrite(AIN2, HIGH);

          digitalWrite(BIN1, LOW);
          digitalWrite(BIN2, HIGH);

          analogWrite(PWMA, speed/2);
          analogWrite(PWMB, speed);
          Serial.println(" FORWARD-RIGHT");
          break;

          case 'H': 
          digitalWrite(AIN1, HIGH);
          digitalWrite(AIN2, LOW);

          digitalWrite(BIN1, HIGH);
          digitalWrite(BIN2, LOW);

          analogWrite(PWMA, speed);
          analogWrite(PWMB, speed/2);
          Serial.println(" BACK-LEFT");
          break;

          case 'J': 
          digitalWrite(AIN1, HIGH);
          digitalWrite(AIN2, LOW);

          digitalWrite(BIN1, HIGH);
          digitalWrite(BIN2, LOW);

          analogWrite(PWMA, speed/2);
          analogWrite(PWMB, speed);
          Serial.println(" BACK-RIGHT");
          break;

      case 'S':
          analogWrite(PWMA, 0);
          analogWrite(PWMB, 0);
          Serial.println(" STOP");
          break;
  }
  }
}





