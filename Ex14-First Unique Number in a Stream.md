# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE: 10.07.2026
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1. Import the necessary Libraries.
2. Initialize a LinkedHashMap and an ArrayList.
3. Input the given element into the map and also its number of occurance using getOrDefualt(N,0)+1
4.  If the number of occrance is 1, then it is a unique number 
5.  Display the unique number

## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.*;

public class FirstUniqueNumberStream {

    public static void processStream(int n, Scanner sc) {
        Map<Integer, Integer> lhm = new LinkedHashMap<>();
        List<Integer> li = new ArrayList<>();
        for(int i=0;i<n;i++)
        {
            boolean flag = true;
            int N = sc.nextInt();
            lhm.put(N,lhm.getOrDefault(N,0)+1);
            li.add(N);            
            for(Integer value : li)
            {
                if(lhm.get(value)==1)
                {
                    flag = false;
                    System.out.println("First unique number: " + value);
                    break;
                }
            }
            if(flag)
                System.out.println("No unique number");
            
        }
        

    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        processStream(n, sc);
        sc.close();
    }
}

```

## Output:

<img width="747" height="550" alt="output Day4" src="https://github.com/user-attachments/assets/871c3411-1d32-4b50-9cd1-9fa70c99db4f" />


## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
