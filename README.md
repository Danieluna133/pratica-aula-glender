# pratica-aula-glender

- Faça um programa que calcule o fatorial de um numero informado pelo usuario:

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */
package javaapplication4;

import java.util.Scanner;

/**
 *
 * @author danal
 */
public class JavaApplication4 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Digite um número inteiro não negativo: ");
        int numero = scanner.nextInt();
        
        // Fatorial de 0 é 1, e não existe fatorial de número negativo
        if (numero < 0) {
            System.out.println("Erro: O número deve ser não negativo.");
        } else {
            long fatorial = 1;
            // Cálculo do fatorial usando laço for
            for (int i = 1; i <= numero; i++) {
                fatorial *= i;
            }
            System.out.println("O fatorial de " + numero + " é: " + fatorial);
        }
    }
    
}


- Faça um programa que diga quantos são os os multiplos de 2,3 e 5 entre 1 e 1000


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */
package atividade.em.sala.pkg02;

/**
 *
 * @author User
 */
public class AtividadeEmSala02 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
       System.out.println("Múltiplos de 2, 3 e 5 entre 1 e 1000:\n");

        for (int i = 1; i <= 1000; i++) {
            
            if (i % 2 == 0 && i % 3 == 0 && i % 5 == 0) {
                System.out.println("Número: " + i + " (Múltiplo comum)");
            } 
            
                System.out.print(i + " ");
            }
    }
    
}
