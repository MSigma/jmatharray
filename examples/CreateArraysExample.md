```java

import org.math.array.util.*;
 
import static java.lang.Math.*;
 
import static org.math.array.DoubleArray.*;
 
public class CreateArraysExample {
        public static void main(String[] args) {
 
                // Id matrix
                double[][] A = identity(5);
 
                // 10 x 5 one matrix
                double[][] B = one(3, 4);
                
                // increment vector : {0,0.1,0.2,0.3,0.4,0.5}
                double[] C = increment(0.0, 0.1, 0.5);
 
                // function of an array : sin(C)
                Function sinus = new Function() {
                        public double f(double x) {
                                return sin(x);
                        }
                };
                double[] D = f(C, sinus);
                
                // print matrices in command line
                System.out.println("A = \n"+tostring(A));
                System.out.println("B = \n"+tostring(B));
                System.out.println("C = \n"+tostring(C));
                System.out.println("D = \n"+tostring(D));
 
        }
}
```
