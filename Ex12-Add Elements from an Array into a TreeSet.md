# Ex12 Add Elements from an Array into a TreeSet
## DATE: 08.07.2026
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Import the necessary Libraries.
2. Create a TreeSet and insert the given element into the TreeSet.
3. Display the TreeSet for sorted order.   

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        TreeSet<Integer> ts = new TreeSet<>();
        for(int a : arr)
        {
            ts.add(a);
        }
        return ts;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}


```

## Output:

<img width="688" height="527" alt="output Day2" src="https://github.com/user-attachments/assets/2b199bc5-2b86-4d23-b043-749958a31f33" />


## Result:
The program successfully adds elements from an array into a TreeSet.
