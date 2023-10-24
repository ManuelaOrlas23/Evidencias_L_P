<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 

# Actividad: Prueba, ejecución y explicación de ejercicios de lógica de programación.

Selecciona dos ejercicios de la sesión 10, impleméntalos, ejecútalos y proporciona una explicación detallada de cada uno.

## - Cálculo del índice de masa corporal (IMC)
El índice de masa corporal (IMC) es una medida que se utiliza para evaluar si una persona tiene un peso saludable en relación con su altura. Se calcula dividiendo el peso de una persona en kilogramos entre el cuadrado de su altura en metros (kg/m²).

El IMC es una herramienta útil para determinar si una persona tiene un peso saludable, está por debajo de su peso ideal o tiene sobrepeso o obesidad. Aunque el IMC no mide directamente la cantidad de grasa corporal, se ha encontrado que existe una relación entre el IMC y el porcentaje de grasa corporal. Por lo tanto, el IMC se utiliza como un indicador general de la salud y el riesgo de ciertas enfermedades relacionadas con el peso, como la diabetes, la hipertensión y las enfermedades cardiovasculares.

Los valores del IMC se interpretan según las siguientes categorías: Bajo peso: IMC menor a 18,5 Peso normal: IMC entre 18,5 y 24,9 Sobrepeso: IMC entre 25 y 29,9 Obesidad grado 1: IMC entre 30 y 34,9 Obesidad grado 2: IMC entre 35 y 39,9 Obesidad grado 3: IMC igual o mayor a 40

Es importante tener en cuenta que el IMC es una herramienta de evaluación general y que no tiene en cuenta otros factores importantes, como la edad, el género, la composición corporal y la distribución de la grasa corporal. Por lo tanto, es recomendable que una evaluación más completa sea realizada por un profesional de la salud.

- Ejemplo en Java de cómo calcular el índice de masa corporal (IMC) de una persona:

```
import java.util.Scanner;

public class IMC {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double weight, height, imc;
      
      // Solicita el peso y la altura
      System.out.print("Ingrese su peso en kilogramos: ");
      weight = input.nextDouble();
      System.out.print("Ingrese su altura en metros: ");
      height = input.nextDouble();

      // Calcula el IMC
      imc = weight / (height * height);

      // Muestra el resultado en la consola
      System.out.printf("Su IMC es %.2f", imc);
   }
}
```

- En este programa, primero se solicita al usuario que ingrese su peso en kilogramos y su altura en metros. Luego se calcula el IMC dividiendo el peso entre la altura al cuadrado. Finalmente, se muestra el resultado en la consola con dos decimales utilizando el método printf de la clase System.out.


 ## -  Calcular la cantidad de materiales necesarios para construir una pared de ladrillos
Cálculo de la cantidad de materiales para la construcción: Este ejercicio consiste en calcular la cantidad de materiales necesarios para construir una estructura. Para ello, se debe tener en cuenta las dimensiones de la estructura y la cantidad de materiales necesarios por unidad de área o de volumen. Algunos ejemplos de cálculos de materiales son el cálculo de la cantidad de ladrillos necesarios para construir una pared, o el cálculo de la cantidad de concreto necesario para una losa o columna.

- Ejemplo en Java de cómo calcular la cantidad de materiales necesarios para construir una pared de ladrillos:

import java.util.Scanner;

public class CantidadLadrillos {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double largo, alto, ancho, areaPared, cantidadLadrillos, largoLadrillo, altoLadrillo, anchoLadrillo;
      
      // Solicita las dimensiones de la pared
      System.out.print("Ingrese el largo de la pared en metros: ");
      largo = input.nextDouble();
      System.out.print("Ingrese el alto de la pared en metros: ");
      alto = input.nextDouble();
      System.out.print("Ingrese el ancho de la pared en metros: ");
      ancho = input.nextDouble();

      // Solicita las dimensiones del ladrillo
      System.out.print("Ingrese el largo del ladrillo en metros: ");
      largoLadrillo = input.nextDouble();
      System.out.print("Ingrese el alto del ladrillo en metros: ");
      altoLadrillo = input.nextDouble();
      System.out.print("Ingrese el ancho del ladrillo en metros: ");
      anchoLadrillo = input.nextDouble();

      // Calcula el área de la pared y del ladrillo
      areaPared = largo * alto;
      double areaLadrillo = largoLadrillo * altoLadrillo;

      // Calcula la cantidad de ladrillos necesarios
      cantidadLadrillos = Math.ceil(areaPared / (areaLadrillo * ancho / anchoLadrillo));

      // Muestra el resultado en la consola
      System.out.printf("Para construir la pared se necesitan %.0f ladrillos.", cantidadLadrillos);
   }
}

- El objetivo de este ejercicio es crear un programa en Java que permita calcular la cantidad de ladrillos necesarios para construir una pared con dimensiones específicas, utilizando ladrillos con dimensiones también específicas.
<!-- Su documentación aquí -->





