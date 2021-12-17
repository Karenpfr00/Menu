# Menu
Menu simples de excercício

import java.util.Scanner;

public class menu {

    public static void main(String[] args) {

        int opcao;
        do {
            System.out.println("|   MENU          |");
            System.out.println("|  Opções:        |");
            System.out.println("|     1. Opção 1  |");
            System.out.println("|     2. Opção 2  |");
            System.out.println("|     3. Sair     |");
            Scanner menu = new Scanner(System.in);

            System.out.println("Selecione uma opção: ");
            opcao = menu.nextInt();

            processar(opcao);
        } while (opcao != 3);
    }

 public static  void processar( int opcao){
     switch (opcao) {
         case 1 -> System.out.println("Opção 1 selecionada");
         case 2 -> System.out.println("Opção 2 selecionada");
         case 3 -> System.out.println("Sair");
         default -> System.out.println("Seleção inválida");
     }
        }
    }