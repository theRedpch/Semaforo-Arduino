# Semaforo-Arduino
En esta primera clase veremos como crear un semaforo en arduino

## Variables

    int led_rojo = 11;
    int led_amarillo = 12;
    int led_verde = 13;
    int boton = 2;

## Setup

    
void setup() {
  // put your setup code here, to run once:
  pinMode(led_rojo, OUTPUT);
  pinMode(led_amarillo, OUTPUT);
  pinMode(led_verde, OUTPUT);
  pinMode(boton, INPUT);
}
