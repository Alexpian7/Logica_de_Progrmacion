<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


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

´´´

## Explicación

> se importa la clase Scanner, se crean la variables de tipo double para leer números decimales.
>El system.out.print es para que el usuario ingrese sus datos
>luego se claculan los datos ingresados por el usuario.

´´´
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
      System.out.print("Ingrese el largo del ladrillo en centimetros: ");
      largoLadrillo = input.nextDouble();
      System.out.print("Ingrese el alto del ladrillo en centimetros: ");
      altoLadrillo = input.nextDouble();
      System.out.print("Ingrese el ancho del ladrillo en centimetros: ");
      anchoLadrillo = input.nextDouble();

      // Calcula el área de la pared y del ladrillo
      areaPared = largo * alto;
      double areaLadrillo = largoLadrillo * altoLadrillo;

      // Calcula la cantidad de ladrillos necesarios
      cantidadLadrillos = Math.ceil(areaPared / ((areaLadrillo * ancho) / anchoLadrillo));

      // Muestra el resultado en la consola
      System.out.printf("Para construir la pared se necesitan %.0f ladrillos.", cantidadLadrillos);
   }
}
´´´

## Explicación

>Se le pide al usuario que ingrese sus datos mediante un System.out,print y se leen con un input.nextDouble.
>Se clacula el area de la pared que es igual al largo por el alto.
>se calcula es area del ladrillo que es igual a largo y alto del ladrillo.
>para calcular la cantidad de ladrillos se crea la funcion math.ceil que devuelve el numero entero mas cercano y luego se multiplica el area delladrillo con el ancho y se divide por el ancho del ladrillo y luego ese resultado se divide por el area de la pared.



