# PRIMER_REPO

Hola esto es una prueba

EJERCICIO 1. 

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num1, num2, num3, menor;

        System.out.print("Ingrese el primer número: ");
        num1 = sc.nextInt();
        System.out.print("Ingrese el segundo número: ");
        num2 = sc.nextInt();
        System.out.print("Ingrese el tercer número: ");
        num3 = sc.nextInt();

        menor = num1;
        if (num2 < menor) {
            menor = num2;
        }
        if (num3 < menor) {
            menor = num3;
        }

        System.out.println("El número menor es: " + menor);
    }
}
EJERCICIO 2.
 
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String frase;
        char letra;
        int contador = 0;

        System.out.print("Ingrese una frase: ");
        frase = sc.nextLine();
        System.out.print("Ingrese una letra: ");
        letra = sc.next().charAt(0);

        for (int i = 0; i < frase.length(); i++) {
            if (frase.charAt(i) == letra) {
                contador++;
            }
        }

        System.out.println("La letra '" + letra + "' aparece " + contador + " veces en la frase '" + frase + "'.");
    }
}

EJERECICIO 7.
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int hora, minutos, segundos;

        System.out.print("Ingrese la hora (formato: hh): ");
        hora = sc.nextInt();
        System.out.print("Ingrese los minutos (formato: mm): ");
        minutos = sc.nextInt();
        System.out.print("Ingrese los segundos (formato: ss): ");
        segundos = sc.nextInt();

        if (hora >= 0 && hora <= 23) {
            if (minutos >= 0 && minutos <= 59) {
                if (segundos >= 0 && segundos <= 59) {
                    System.out.println("La hora es válida.");
                } else {
                    System.out.println("Los segundos no son válidos.");
                }
            } else {
                System.out.println("Los minutos no son válidos.");
            }
        } else {
            System.out.println("La hora no es válida.");
        }
    }
}

EJERECICIO 8.

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int mes;
        String nombreMes = "";
        int dias = 0;
        
        System.out.print("Ingrese el número del mes (1-12): ");
        mes = sc.nextInt();

        switch (mes) {
            case 1:
                nombreMes = "Enero";
                dias = 31;
                break;
            case 2:
                nombreMes = "Febrero";
                dias = 28;
                break;
            case 3:
                nombreMes = "Marzo";
                dias = 31;
                break;
            case 4:
                nombreMes = "Abril";
                dias = 30;
                break;
            case 5:
                nombreMes = "Mayo";
                dias = 31;
                break;
            case 6:
                nombreMes = "Junio";
                dias = 30;
                break;
            case 7:
                nombreMes = "Julio";
                dias = 31;
                break;
            case 8:
                nombreMes = "Agosto";
                dias = 31;
                break;
            case 9:
                nombreMes = "Septiembre";
                dias = 30;
                break;
            case 10:
                nombreMes = "Octubre";
                dias = 31;
                break;
            case 11:
                nombreMes = "Noviembre";
                dias = 30;
                break;
            case 12:
                nombreMes = "Diciembre";
                dias = 31;
                break;
            default:
                System.out.println("El mes ingresado es inválido");
                break;
        }

        if (dias > 0) {
            System.out.println(nombreMes + " tiene " + dias + " días.");
        }
    }
}



