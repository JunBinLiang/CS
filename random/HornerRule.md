Given a polynomial of the form cnxn + cn-1xn-1 + cn-2xn-2 + … + c1x + c0 and a value of x, find the value of polynomial for a given value of x. Here cn, cn-1, .. are integers (may be negative) and n is a positive integer.
Input is in the form of an array say poly[] where poly[0] represents coefficient for xn and poly[1] represents coefficient for xn-1 and so on.
Examples: 

// Evaluate value of 2x3 - 6x2 + 2x - 1 for x = 3
Input: poly[] = {2, -6, 2, -1}, x = 3
Output: 5

// Evaluate value of 2x3 + 3x + 1 for x = 2
Input: poly[] = {2, 0, 3, 1}, x = 2
Output: 23



Horner’s method can be used to evaluate polynomial in O(n) time. 
To understand the method, let us consider the example of 2x3 – 6x2 + 2x – 1. 
The polynomial can be evaluated as ((2x – 6)x + 2)x – 1. 


```

// Java program for implementation of Horner Method
// for Polynomial Evaluation
import java.io.*;
 
class HornerPolynomial
{
    // Function that returns value of poly[0]x(n-1) +
    // poly[1]x(n-2) + .. + poly[n-1]
    static int horner(int poly[], int n, int x)
    {
        // Initialize result
        int result = poly[0]; 
  
        // Evaluate value of polynomial using Horner's method
        for (int i=1; i<n; i++)
            result = result*x + poly[i];
  
        return result;
    }
     
    // Driver program
    public static void main (String[] args)
    {
        // Let us evaluate value of 2x3 - 6x2 + 2x - 1 for x = 3
        int[] poly = {2, -6, 2, -1};
        int x = 3;
        int n = poly.length;
        System.out.println("Value of polynomial is "
                                        + horner(poly,n,x));
    }
}
 
// Contributed by Pramod Kumar
```
