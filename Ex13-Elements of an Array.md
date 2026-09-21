# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE: 08.07.2026
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Import the necessary utilities.
2. Initialize an array with the give size.
3. Input the value to be filled.1
4. Use Arrays.fill() utility to fill the array with constant value.


## Program:
```
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.*;

public class FillArrayUsingArraysFill {

    public static int[] fillArray(int size, int value) {
       
        int[] arr = new int[size];
        Arrays.fill(arr,value);
        return arr;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int value = sc.nextInt();
        int[] arr = fillArray(10, value);
        System.out.println("Array elements:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}

```

## Output:

<img width="790" height="250" alt="output Day3" src="https://github.com/user-attachments/assets/6ee6528b-3c23-4d8d-b76e-e01bd77af3b1" />


## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
