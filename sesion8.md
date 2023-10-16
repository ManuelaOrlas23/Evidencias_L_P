<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 

### Actividad: Ejecicios de métodos en Java

- Implementar los siguientes métodos:

1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.
2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.
3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.
4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.
5. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

### Desarrollo

1. 
```
public class MayorDeDosNumeros {
    public static int encontrarMayor(int num1, int num2) {
        if (num1 > num2) {
            return num1;
        } else {
            return num2;
        }
    }
    public static void main(String[] args) {
        int numero1 = 10;
        int numero2 = 20;
        int resultado = encontrarMayor(numero1, numero2);
        System.out.println("El número mayor es: " + resultado);
    }
}
```
2. 
```
public class ContadorDeVocales {
    public static int contarVocales(String texto) {
        int contador = 0;
        for (int i = 0; i < texto.length(); i++) {
            char caracter = texto.charAt(i);
            if (caracter == 'a' || caracter == 'e' || caracter == 'i' || caracter == 'o' || caracter == 'u' ||
                caracter == 'A' || caracter == 'E' || caracter == 'I' || caracter == 'O' || caracter == 'U') {
                contador++;
            }
        }
        return contador;
    }
    public static void main(String[] args) {
        String texto = "Escribe un método que cuente las vocales en una cadena de texto.";
        int resultado = contarVocales(texto);
        System.out.println("El número de vocales en el texto es: " + resultado);
    }
}
```
3. 

4. 
```
public class ContadorDePalabras {
    public static int contarPalabras(String texto) {
        // Divide la cadena en palabras utilizando espacios en blanco como delimitador
        String[] palabras = texto.split("\\s+");
        // El tamaño del arreglo "palabras" es igual al número de palabras
        return palabras.length;
    }
    public static void main(String[] args) {
        String texto = "Este es un ejemplo de contador de palabras en Java.";
        int resultado = contarPalabras(texto);
        System.out.println("El número de palabras en el texto es: " + resultado);
    }
}
```
5. 

```
import java.util.Arrays;
public class OrdenarPalabrasAlfabeticamente {
    public static String ordenarPalabras(String texto) {
        
        String[] palabras = texto.split("\\s+");
        
        
        Arrays.sort(palabras);
        
        
        String resultado = String.join(" ", palabras);
        
        return resultado;
    }
    public static void main(String[] args) {
        String texto = "Este es un ejemplo de ordenar palabras alfabéticamente en Java";
        String resultado = ordenarPalabras(texto);
        System.out.println("Texto con palabras ordenadas alfabéticamente: " + resultado);
    }
}
```

<!-- Su documentación aquí -->






