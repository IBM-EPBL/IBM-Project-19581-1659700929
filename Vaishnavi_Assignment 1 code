# IBM-Project-19581-1659700929
Smart Solutions For Railways
Assignment 1 code is given:
#define LED_RED 10
#define BUZZER 6
int sensorValue=0;
#include<Servo.h>
Servo Myservo;
void setup()
{
   Serial.begin(9600);
   pinMode(A0, INPUT);
   pinMode(LED_RED, OUTPUT);
   pinMode(BUZZER, OUTPUT);
   Myservo.attach(11);
}

void loop()
{
  
  sensorValue=digitalRead(A0)*500;
  Serial.print(" ");
  Serial.println(sensorValue);
  if(sensorValue<500)
  {
    digitalWrite(LED_RED, HIGH);
    tone(BUZZER,900);       //FREQUENCY IN HERTZ
    Myservo.write(0);
    delay(50);             //ms
  }
  else(sensorValue>499);
  digitalWrite(LED_RED, LOW);
  noTone(BUZZER);
  Myservo.write(180);
}

This assignment demonstrates the usage of sensor like tilt sensor, which acts as a tilt in the vehicle. The servo motor records the movement and urges the buzzer to beep, indicating that a theft is happening.



