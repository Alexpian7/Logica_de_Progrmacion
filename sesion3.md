<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


### Ejer1

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejer2;

/**
 *
 * @author Anderson Alzate
 */

import java.util.Scanner;

public class Ejer2 {

    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);
        
        System.err.println("Ingrese su primer numero: ");
        int num1 = scanner.nextInt();
        
        System.err.println("Ingrese su segundo numero: ");
        int num2 = scanner.nextInt();
        
        System.out.println( "La suma es: " + (num1 + num2));  
       
        System.out.println( "La multiplicacion es: " + (num1 * num2));  
        
        
    }
}

```
### ejer2

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejer2;

/**
 *
 * @author Anderson Alzate
 */

import java.util.Scanner;

public class Ejer2 {

    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);
        
        System.err.println("Ingrese su primer numero: ");
        int num1 = scanner.nextInt();
        
        System.err.println("Ingrese su segundo numero: ");
        int num2 = scanner.nextInt();
       
        System.out.println( "La resta es: " + (num1 - num2));  
       
        System.out.println( "La divixion es: " + (num1 / num2)); 
        
        
    }
}

```
### Ejer3

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejer3;

/**
 *
 * @author Anderson Alzate
 */
import java.util.Scanner;

public class Ejer3 {

    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);
        
        System.err.println("Ingrese su primer numero: ");
        int num1 = scanner.nextInt();
        
        System.err.println("Ingrese su segundo numero: ");
        int num2 = scanner.nextInt();
        
        if(num1 < num2){
        System.out.println( "El numero menor es : " + num1);  
        }
        else {
            if(num1 > num2){
              System.out.println( "El numero mayor es : " + num1);   
            }
            else {
                if(num1 == num2){
                    System.out.println( "Los numeros son iguales"); 
                }
            }
        }
       
        
    }
    }
```

### Ejer4

```
package com.mycompany.ejer4;

import java.util.Scanner;
public class Ejer4 {

    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);
  
        
 
        int num=1;
 
        //Definimos el bucle, incluye el 100
        while (num<=100){
            System.out.println(num);
            //Incrementamos num
            num++;
        }
    }
}
```

### Ejer5

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejer5;

import java.util.Scanner;

/**
 *
 * @author Anderson Alzate
 */
public class Ejer5 {

    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);
        int n =  4;
        i = 0;
        for(i = 0 > n = 4)
            System.out.println( "Lo siento, usted no es apto para votar");  
        
    }
}
```

### Ejer6

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */
package com.mycompany.ejer6;

/**
 *
 * @author Anderson Alzate
 */
import java.util.Scanner;

public class Ejer6 {

    public static void main(String[] args) {
        
         Scanner scanner = new Scanner(System.in);

         System.err.println("Ingrese su primer numero: ");
        double num1 = scanner.nextDouble();
        
        System.err.println("Ingrese su segundo numero: ");
        double num2 = scanner.nextDouble();
        
        System.out.println( "La suma es: " + (num1 + num2));  
        System.out.println( "La resta es: " + (num1 - num2));  
        System.out.println( "La multiplicacion es: " + (num1 * num2));  
        System.out.println( "La divixion es: " + (num1 / num2));  
```

### Ejer7

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */
package com.mycompany.ejer7;

/**
 *
 * @author Anderson Alzate
 */
import java.util.Scanner;

public class Ejer7 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = 4;
        n++;
      System.out.println(n);
      System.out.println(n - 1);
```





