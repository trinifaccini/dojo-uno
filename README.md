# DOJO NUMERO UNO - GRUPO F

![Tinkercard](https://github.com/trinifaccini/dojo-uno/blob/main/img/DOJO-UNO-GRUPO-F-ENTREGA-UNO.png)

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

## Descripción

Creamos un semáforo con señalización para no videntes. 

## Finalidad del proyecto
Demostrar los conocimientos aprendidos en la materia Sistema de Procesamiento de Datos.

## Función principal

Esta función se encarga de hacer sonar al buzzer dos veces por el tiempo recibido por parametro y repite este comportamiento 10 veces. 

intensidad_fuerte es una variable global de tipo entero, que en nuestro caso tiene el valor 250. 

~~~ C++ 

void sonarSilenciarBuzzer(int buzzer, int tiempo)
{
  int contador = 0;
  
  while (contador < 10)
  {
    sonarBuzzer(buzzer, tiempo, intensidad_fuerte);
    silenciarBuzzer(buzzer, tiempo);
    sonarBuzzer(buzzer, tiempo, intensidad_fuerte);
    silenciarBuzzer(buzzer, tiempo);
    contador = contador + 1;
  }
}
~~~

## :robot: Link al proyecto
- [Tinkercard-Sol Rubinetti](https://www.tinkercad.com/things/iZNwefUZfGa-dojo-1-grupo-f-clase-5/editel?sharecode=4DJUVY-ezPfkTXRP7us0aNPnXKNrvgEcs_NTCFw-zh4)
- [Tinkercard-Yamila Sueldo](https://www.tinkercad.com/things/ekHG25jeY0k-dojo-numero-uno/editel?sharecode=_ZBsYcqE1y3GENhjB3fzVXFeKbKeGMpGsUccB4qW-Ok)
- [Tinkercard-Adrian Barrientos](https://www.tinkercad.com/things/8mgCsJsUrRK-bodacious-borwo/editel?sharecode=VCCzrcbr8gq2P9JAjRSaL-b77EM1lVzc9hE01hZxCX8)
- [Tinkercard-Lautaro Torres](https://www.tinkercad.com/things/fSOhHiGeVdJ-ejercicio-dojo-1-1/editel?sharecode=9IKDJYqicsguvunn1_dn7oklyXOUMo9TCehS7j1dNF8)
- [Tinkercard-Trinidad Faccini](https://www.tinkercad.com/things/3WUXu8RRyCe-dojo-uno-grupo-f-entrega-uno/editel?sharecode=auH-Hu3eBpDSPj273IRXl5Y4IbzwZkOZd1af6DUXJGE)
