<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 


´´´

package com.mycompany.array;

/**
 *
 * @author Anderson Alzate
 */
public class Array {

    public static void main(String[] args) {
          Integer [] arr = new Integer [] {1, 2, 3, 4, 2, 7, 8, 8, 3, 3, 10, 11, 15, 1, 3, 3};
    String repetidos = "";
    boolean imprimeComa = false; 

    System.out.println("Elementos duplicados en arr: "); 

    // Busca los duplicados 
    for (int i = 0; i < arr.length; i++) {  
       for (int j = i + 1; j < arr.length; j++) {
          // Comprobamos si i igual a j y si aún no está en "repetidos"
          if (
               arr[i].equals(arr[j]) 
               && 
               !repetidos.contains("*" + arr[i].toString() + "*") 
          ) {

             if (!imprimeComa){
                imprimeComa = true;
             } else {
                repetidos += ", "; 
             }

             // Imprime los elementos duplicados
             repetidos += "*" + arr[j] + "*";
          }
       }
    }
´´´

´´´
package com.mycompany.araylist;
import java.util.Scanner;



        

/**
 *
 * @author Anderson Alzate
 */
public class ArayList {
    
  

    public static void main(String[] args) {
       Scanner input = new Scanner(System.in);
   int numeroDecimal = 10;

        // Declaramos la variable para almacenar el resultado
        String numeroBinario = "";

        // Inicializamos el bucle
        int i = 0;
        while (numeroDecimal > 0) {

            // Calculamos el resto de la división
            int resto = numeroDecimal % 2;

            // Añadimos el resto a la cadena
            numeroBinario = resto + numeroBinario;

            // Dividimos el número decimal por 2
            numeroDecimal = numeroDecimal / 2;

            // Incrementamos el índice del bucle
            i++;
        }

        // Imprimimos el resultado
        System.out.println("El número binario es: " + numeroBinario);
    }
}
´´´

## Solución 2

´´´
package com.mycompany.array;
import java.util.Scanner;
/**
 *
 * @author Anderson Alzate
 */
public class Array {

    public static void main(String[] args) {
     long numero, aux, digito, decimal;
     int exponente;
     boolean esBinario;
     Scanner sc = new Scanner(System.in);

    //Leer un número por teclado y comprobar que es binario
     do {
          System.out.print("Introduce un numero binario: ");
          numero = sc.nextLong();
          //comprobamos que sea un número binario es decir
          //que este formado solo por ceros y unos
          esBinario = true;
          aux = numero;
          while (aux != 0) {
                     digito = aux % 10; //última cifra del números
                     if (digito != 0 && digito != 1) { //si no es 0 ó 1
                          esBinario = false; //no es un número binario
                     }
                     aux = aux / 10; //quitamos la última cifra para repetir el proceso                           
           }
      } while (!esBinario); //se vuelve a pedir si no es binario

      //proceso para pasar de binario a decimal
      exponente = 0;
      decimal = 0; //será el equivalente en base decimal
      while (numero != 0) {
                //se toma la última cifra
                digito = numero % 10;
                //se multiplica por la potencia de 2 correspondiente y se suma al número                          
                decimal = decimal + digito * (int) Math.pow(2, exponente);
                //se aumenta el exponente
                exponente++;
                //se quita la última cifra para repetir el proceso
                numero = numero / 10;
      }
      System.out.println("Decimal: " + decimal);
    }
}
´´´



