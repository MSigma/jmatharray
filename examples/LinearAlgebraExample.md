```java


import static org.math.array.LinearAlgebra.*;
 
public class LinearAlgebraExample {
        public static void main(String[] args) {
 
                // random 4 x 3 matrix
                double[][] A = random(4, 3);
 
                // random 4 x 3 matrix
                double[][] B = random(4, 3);
 
                // random 4 x 4 matrix + Id
                double[][] C = plus(random(4, 4),identity(4));
                
                // linear algebra
                double[][] D = plus(A, B);
 
                double[][] E = plus(A, 1);
 
                double[][] F = minus(A, B);
 
                double[][] G = minus(2, A);
                
                double[][] H = times(A, transpose(B));
 
                double[][] I = times(A, 10);
 
                double[][] J = divide(C, B);
 
                double[][] K = divide(A, 10);
 
                double[][] L = inverse(C);
 
                // print matrices in command line
                System.out.println("A = \n" + tostring(A));
                System.out.println("B = \n" + tostring(B));
                System.out.println("C = \n" + tostring(C));
                System.out.println("D = A + B = \n" + tostring(D));
                System.out.println("E = A + 1 = \n" + tostring(E));
                System.out.println("F = A - B = \n" + tostring(F));
                System.out.println("G = 2 - A = \n" + tostring(G));
                System.out.println("H = A * t(B) = \n" + tostring(H));
                System.out.println("I = A * 10 = \n" + tostring(I));
                System.out.println("J = C / B = \n" + tostring(J));
                System.out.println("K = A / 10 = \n" + tostring(K));
                System.out.println("L = C^-1 = \n" + tostring(L));
 
        }
}


```
