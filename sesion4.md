<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Project/Maven2/JavaApp/src/main/java/${packagePath}/${mainClassName}.java to edit this template
 */
package com.mycompany.ejer10;

import java.util.Scanner;

/**
 *
 * @author CESDE Determinar si el estudiante tiene una beca o una carrera
 * relacionada con el desarrollo de software.
 */
public class Ejer10 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String nombre = "Juan Pérez";
        String apellido = "González";
        String identificación = "1000000001";
        String correo = "juan.perez@ejemplo.com";
        String carrera = "Desarrollo de Software";
        String universidad = "Cesde";

// Variable de tipo int
        System.err.println("Ingrese su Edad: ");
        int edad = scanner.nextInt();
// Variable de tipo boolean
        boolean esActivo = true;
        boolean becado = true;
// Variable de tipo char
        char género = 'M';
// Variable de tipo double
        double promedio = 4.5;
// Variable de tipo int
        int semestre = 2;

        if (edad >= 18 && esActivo) {
            System.out.println(" El estudiante es mayor de edad y tiene estado Activo");
        } else {
            System.out.println(" El estudiante no esta Activo y ");
        }
        if (carrera.equals("Desarrollo de Software") || becado) {
            System.out.println("El estudiante tiene una carrera de: " + carrera);
        } else {
            System.out.println("El estudiante tiene una beca: " + becado);
        }
        if (semestre == 2 && esActivo) {
            System.out.println("El estudiante esta en el ultimo semestre y tiene un estado Activo");
        } else {
            System.out.println("El estudiante no esta en el ultimo semestre y no esta activo ");
        }
        if (carrera.equals("Desarrollo de Software") && promedio >= 4.5) {
            System.out.println("El estudiante esta en la carrera de Desarrollo de Software y tiene un promedio superior y ");
        } else {
            System.out.println("El estudiante tiene un premdio por debajo a 4.5");
        }
        System.out.println("El estudiante " + nombre + " " + apellido + " " + "identificado con # de documento " + identificación);
        System.out.println("Correo " + correo + " " + " y carrera " + carrera + " " + "estudia en la universidad " + universidad);

        if (universidad.equals("Cesde") && promedio == 4.5 && esActivo) {

            System.out.println("El estudiante tiene una beca del 50%");
        } else {
            System.out.println("El estudiante no puede acceder a la beca");
        }

        if (promedio >= 0.0 && promedio <= 3.4) {
            System.out.println("El estudiante no puede acceder a la beca");
        } else {
            if (promedio >= 3.5 && promedio <= 3.9) {
                System.out.println("El estudiante recibe una beca parcial del 25%");
            } else {
                if (promedio >= 4.0 && promedio <= 4.5) {
                    System.out.println(" El estudiante recibe una beca parcial del 50%.");
                } else {
                    if (promedio >= 4.5 && promedio <= 5.0) {
                        System.out.println(" El estudiante recibe una beca completa..");
                    }
                }
            }
        }

    }
}

```






