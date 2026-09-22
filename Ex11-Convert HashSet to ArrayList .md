# Ex11 Convert HashSet to ArrayList in Java
## DATE: 08.08.2026
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1. Import the necessary Libraries.
2. Create a method to convert a HashSet into ArrayList.
3. Create a HashSet.
4. Insert the elements into HashSet.
5. Display the ArrayList

## Program:
```
/*
Program to To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.*;

public class HashSetToArrayList {

    public static ArrayList<Integer> convertToArrayList(HashSet<Integer> set) {
        ArrayList<Integer> al = new ArrayList<>();
        for(Integer a : set)
            al.add(a);
            
        return al;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            set.add(num);
        }

        ArrayList<Integer> list = convertToArrayList(set);
        System.out.println("ArrayList contents:");
        for (int num : list) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}


```

## Output:

<img width="680" height="657" alt="output Day1" src="https://github.com/user-attachments/assets/1d98ffc5-f298-43a7-b8e1-bf18dee1159c" />


## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
