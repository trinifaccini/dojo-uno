# DOJO NUMERO UNO - GRUPO F

## Integrantes 
- Sol Rubinetti
- Yamila Sueldo
- Adrian Barrientos
- Lautaro Torres
- Trinidad Faccini

## Consigna
El gobierno de la ciudad quiere actualizar los semáforos que tiene instalados. La empresa  “UTNFRA Robotics” ganó la licitación y ahora les toca a los desarrolladores de la empresa generar  un proyecto low cost que cumpla con las especificaciones que el gobierno de la ciudad nos  impone, a saber las especificaciones son las siguientes. 

### Primer entrega:
1. El semáforo tiene que tener 2 leds de cada color como mínimo, en caso de que uno se  rompa. 
2. Tiene que implementar los tiempos correctos como se detallan a continuación. 
3. El verde dura 5 segundos. 
4. El amarillo dura 3 segundos. 
5. Rojo dura 5 segundos. 
6. Tiene que tener señalización para personas no videntes como se detalla a  continuación. (Buzzer o piezo)
7. Durante el rojo: Tiene que sonar 2 vez por segundo en un tono FUERTE. 

### Segunda entrega: 
8. Durante el amarillo: Tiene que sonar 1 vez por segundo en un tono SUAVE. 
9. Al cambiar de verde a amarillo debe titilar 3 veces el verde antes de pasar al amarillo
10. Al cambiar de amarillo a rojo se debe titilar 3 veces el amarillo
11. Al cambiar de rojo a Amarillo se debe titilar 3 veces el rojo
12. Al cambiar de amarillo a verde se debe titilar 3 veces el amarillo.

### Tercer entrega: 
13. Agregar un botón (pull down) que al presionarlo se active la funcionalidad de luz verde con más tiempo, dándole a la persona que lo necesite más tiempo para cruzar la calle , sirve para la próxima luz verde y solo para la próxima luz verde después de presionar el botón. el tiempo se duplicará. 
14. Colocar dos semáforos de calles que se crucen  y programarlos para que funcionen en conjunto.

## Descripción/Explicacion
En este parrafo deberan describir que funcion cumple su proyecto. Que solucion esta ofreciendo.

## Finalidad del proyecto

## Función principal


~~~ C++ 
void loop()
{
  Serial.println("Encender luz verde x 5 segundos");
  prenderLed(PIN_LED_VERDE_1);
  prenderLed(PIN_LED_VERDE_2);
  delay(5000);
  Serial.println("Apagar luz verde");
  apagarLed(PIN_LED_VERDE_1);
  apagarLed(PIN_LED_VERDE_2); 
  
  Serial.println("Encender luz amarilla x 3 segundos");
  prenderLed(PIN_LED_AMARILLO_1);
  prenderLed(PIN_LED_AMARILLO_2);
  delay(3000);
  Serial.println("Apagar luz amarilla");

  apagarLed(PIN_LED_AMARILLO_1);
  apagarLed(PIN_LED_AMARILLO_2); 
  
  Serial.println("Encender luz roja x 5 segundos");
  prenderLed(PIN_LED_ROJO_1);
  prenderLed(PIN_LED_ROJO_2);
  
  // ESTA FUNCION DURA 5 SEGUNDOS
  sonarSilenciarBuzzer(PIN_BUZZER, tiempo_buzzer);
 
  Serial.println("Apagar luz roja");
  apagarLed(PIN_LED_ROJO_1);
  apagarLed(PIN_LED_ROJO_2); 
}
~~~

## :robot: Link al proyecto
- [Tinkercard](https://www.tinkercad.com/things/8tPHbv0orHG)
## :tv: Link al video del proceso
- [Video]()







