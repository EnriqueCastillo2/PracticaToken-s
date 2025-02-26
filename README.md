```java
package practicar;

import java.util.Scanner;



public class Practicar {

    
    public static void main(String[] args) throws ClassNotFoundException {
        
        String[] tokens= {"casa","carro","Azul"};
        System.out.println("Ingrese el texto a evaluar");
        String texto = new Scanner(System.in).nextLine();
        
        
        if (palabraRes(tokens,texto)) {
            
        }else {
            System.out.println("no hay palabras reservadas");
        }
                        
      
        }
    
        public static boolean palabraRes(String[] tokens, String texto){
            boolean tienePR=false;
             for (int i = 0; i < tokens.length ;i++) {
             if(texto.contains(tokens[i])){
                 System.out.println( tokens[i] +" es una palabra reservada" );
                tienePR=true;
             }
             }
             return tienePR;
        }
        
}
