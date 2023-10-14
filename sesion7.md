<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


## Actividad: Ejecicios Array - ArrayList

1.  En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList.
Ejemplo Array

´´´
package com.mycompany.array;
import java.util.Arrays;

/*
se debe importa una libreria Arrays para que pueda funcionar
*/

public class Array {

    public static void main(String[] args) {
         int[] numeros = {5, 2, 10, 7, 1};

         /*
         se crea la lista y se le da un valor entero

         */

        // Imprimir el array original
        System.out.println("Array original: " + Arrays.toString(numeros));

        /*
        este codigo me muestra los numeros que tengo dentro del arrays, como lostengo dentro de una cadena debo convertir de string a enteros para que me muestre los numeros.

        */

        // Calcular la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }

        /*
        la variable suma se inicializa desde 0 y los numeros se guardan dentro un contador para que me dar la suma
        */
        System.out.println("La suma de los elementos es: " + suma);

        // Encontrar el número más grande en el array
        int maximo = numeros[0];
        for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
        }

        /*
        la variable i se inicializa desde 1 y va desde 1 menor a numeros.length para que me devuleva numeros enteros, se le agrega un contador y me muestra el numero mayor.
        */
        System.out.println("El número más grande es: " + maximo);

        // Ordenar el array en orden ascendente
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));
    }
}
´´´






