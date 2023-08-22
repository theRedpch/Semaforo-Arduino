![image](https://github.com/theRedpch/Semaforo-Arduino/assets/71972224/0883eb8b-b333-4baa-a1c5-e83f7b3aea58)
# Semaforo-Arduino
En esta primera clase veremos como crear un semaforo en arduino

## Variables

    int led_rojo = 11;
    int led_amarillo = 12;
    int led_verde = 13;
    int boton = 2;

## Variables
 
    void setup() {
      pinMode(led_rojo, OUTPUT);
      pinMode(led_amarillo, OUTPUT);
      pinMode(led_verde, OUTPUT);
      pinMode(boton, INPUT);
    }


## Loop

    void loop() {
      // put your main code here, to run repeatedly:
      digitalWrite(led_rojo, HIGH);
      digitalWrite(led_amarillo, LOW);
      digitalWrite(led_verde, LOW);
     if(digitalRead(boton)==HIGH){
      digitalWrite(led_rojo, LOW);
      digitalWrite(led_amarillo, HIGH);
      digitalWrite(led_verde, LOW);
      delay(500);
      digitalWrite(led_rojo, LOW);
      digitalWrite(led_amarillo, LOW);
      digitalWrite(led_verde, HIGH);
      delay(2000); 
     }
    }
