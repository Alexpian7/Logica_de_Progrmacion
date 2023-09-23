<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


### Ejercios While

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */
package com.mycompany.ejer1;

/**
 * 
 *
 * @author Anderson Alzate
 */

import java.util.Scanner;

public class Ejer1 {  

 
    public static void main(String[] args) {
        // Declaración de variables
        Scanner scanner = new Scanner (System.in);
      
     
       int mult = 1;
       
      System.err.println("Ingrese su numero: ");
      int num = scanner.nextInt();
      
      while(mult <= 10){
      System.out.println( num + " " + "x" +" "+ mult + " " + "=" + " " + (num * mult));
      mult++;
      }
      
    }
}
```

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejer11;
import java.util.Scanner;
/**
 *
 * @author Anderson Alzate
 */
public class Ejer11 {

    public static void main(String[] args) {
         Scanner scanner = new Scanner (System.in);
         
         
         System.out.print("Ingrese una cadena de caracteres: ");
        String cadena = scanner.nextLine();

        int i = 0;
        int contadorNumeros = 0;

        while (i < cadena.length()) {
            char caracter = cadena.charAt(i);
            if (Character.isDigit(cadena.charAt(i))) {
                contadorNumeros++;
                caracter+=cadena.charAt(i);
            }
            i++;
        }
        System.out.println("La cadena ingresada contiene " + contadorNumeros + " números.");
    }
}
```

### Ejercios do - While

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */
package com.mycompany.ejer12;

import java.util.Scanner;

/**
 *
 * @author Anderson Alzate
 */
public class Ejer12 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n;

        do {
            System.out.println("1. Ingrese el Número 1 (ingrese un número negativo para parar el progrma): ");
            System.out.println("2. Mostrar los numeros del 1 al 100 : ");
            System.out.println("Intruduce suopción : ");
            n = scanner.nextInt();

            switch (n) {
                case 1:
                    for (n = 0; n <= 100; n++) {

                        System.out.println(n);
                    }
                    break;
                    
                case 2:
                if(n != 1){
                System.out.print("Escriba 1 para mostrar los numeros del 1 al 100, muchas gracias.");
                }
              
            }
            
        }while (n > 0);
    }
}
```

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejer11;
import java.util.Scanner;
/**
 *
 * @author Anderson Alzate
 */
public class Ejer11 {

    public static void main(String[] args) {
         Scanner scanner = new Scanner (System.in);
         
         
         System.out.print("Ingrese una cadena de caracteres: ");
        String cadena = scanner.nextLine();

        int i = 0;
        int contadorNumeros = 0;

        while (i < cadena.length()) {
            char caracter = cadena.charAt(i);
            if (Character.isDigit(cadena.charAt(i))) {
                contadorNumeros++;
                caracter+=cadena.charAt(i);
            }
            i++;
        }
        System.out.println("La cadena ingresada contiene " + contadorNumeros + " números.");
    }
}
```


### Ejercios for

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejer14;
import java.util.Scanner;
/**
 *
 * @author Anderson Alzate
 */
public class Ejer14 {

    public static void main(String[] args) {
         Scanner scanner = new Scanner(System.in);
         
         
         for(int i = 1; i <= 50; i++){
        System.out.println("Los números impares son: "+ i);
        i+=1;
         }
    }
}

```

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */
package com.mycompany.ejer15;

import java.util.Scanner;

/**
 *
 * @author Anderson Alzate
 */
public class Ejer15 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        boolean primo;
        System.out.println("Los números primos del 1 al 100 son: ");

        for (int num = 1; num <= 100; num++) {
            primo = true;
            for (int i = num - 1; i > 1; i--) {
                if (num % i == 0) {
                    primo = false;
                    break;
                }
            }
            if (primo) {
                System.out.println(num + " es primo");
            }
        }
    }

}
```




