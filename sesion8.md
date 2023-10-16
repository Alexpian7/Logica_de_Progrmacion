<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 

1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

´´´
package com.mycompany.araylist;
import java.util.Scanner;

        

/**
 *
 * @author Anderson Alzate
 */
public class ArayList {
    
    static int maximo (int a, int b){
    int max = 0;
    if(a>b)
        max=a;
    else
        if(a<b)
            max=b;
    return max;
    }

    public static void main(String[] args) {
       Scanner sn= new Scanner(System.in);
       int max =0;
       int a=0,b=0;
       System.out.print("Ingrese el primer Numero: ");
       a=sn.nextInt();
       System.out.print("Ingrese el segundo Numero: ");
       b=sn.nextInt();
       
       max = maximo(a,b);
       
       System.out.println("El Máximo es: "+max);
     

    }
}
´´´

2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.

´´´
package com.mycompany.araylist;
import java.util.Scanner;

        

/**
 *
 * @author Anderson Alzate
 */
public class ArayList {
    
  

    public static void main(String[] args) {
       Scanner sn= new Scanner(System.in);
       
       String cadena;
       int contar = 0;
       char letra;
       
      System.out.print("Ingrese una palabra: ");
      cadena = sn.nextLine();
      
      for(int i=0;i<cadena.length();i++){
      letra = Character.toLowerCase(cadena.charAt(i));
      if (letra == 'a' || letra == 'e' || letra == 'i' || letra == 'o' || letra == 'u' ){
      contar++;
      }
      }
       
       System.out.println("La cantiad de vocales son: "+contar);
     

    }
}
´´´

3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

´´´
package com.mycompany.araylist;
import java.util.Scanner;

        

/**
 *
 * @author Anderson Alzate
 */
public class ArayList {
    
  

    public static void main(String[] args) {
       Scanner sn= new Scanner(System.in);
       
       String cadena;
       
       
      System.out.print("Ingrese una palabra: ");
      cadena = sn.nextLine();
      
    System.out.println("La palabra es minusculas es: "+cadena.toLowerCase());
     System.out.println("La palabra es mayusculas es: "+cadena.toUpperCase());
     

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
       Scanner sn= new Scanner(System.in);
       
       String cadena;
       int nletras = 0;
       
      System.out.print("Ingrese una palabra: ");
      cadena = sn.nextLine();
      for(int i = 0; i<cadena.length();i++){
       if(Character.isLetter(cadena.charAt(i)));
       nletras++;
      }
          
     System.out.println("La palabra contiene: "+nletras+" "+"letras.");
     

    }
}

´´´




