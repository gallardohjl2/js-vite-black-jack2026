```java
package mx.edu.uttt.recursividad;

public class Recursividad2 {
    public static void main(String[] args) {
//        int resultado = sumarIterativo(5);
//        System.out.println("La suma es: " + resultado);

        int resultado = sumarRecursivo(4);
        System.out.println("La suma es: " + resultado);
    }

    public static int sumarIterativo(int n) {
        int suma = 0;
        for (int i =1; i <=n; i++) {
            suma+=i; // Acumulación
        }
        return suma;
    }

    public static int sumarRecursivo (int n){
        //Caso Base
        if(n == 1){
            return 1;
        }else{
            return n + sumarRecursivo(n-1);
        }

        /*
        * resultado = 1;
        *             |
        *             return 1
        *                   |
        *             return 1
        *                    |
        *             return 1
        *
        *    resultado = 10 -> main
        *                           |
        *              return  4 + 6
        *                           |
        *              return  6
        *                            |
        *              return  3
        *                           |
        *                          return 1
        * */

    }

    // TODO: Calcular la potencia (2^4 = 2*2*2*2)
}
```