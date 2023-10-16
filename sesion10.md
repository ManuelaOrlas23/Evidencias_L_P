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
<!-- Su documentación aquí -->





