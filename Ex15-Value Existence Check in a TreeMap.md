# Ex15 Value Existence Check in a TreeMap
## DATE: 10.07.2026
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Import the necessary libraries.
2. Initialize a TreeMap and insert the key and value pair into the map.
3. Use the method map.containsValue() to find if the value exists.
4. Display the final result.

## Program:
```
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.*;

public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        if(map.containsValue(searchValue))
            System.out.printf("Value \"%s\" exists in the TreeMap.",searchValue);
        else
            System.out.printf("Value \"%s\" does not exist in the TreeMap.",searchValue);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}

```

## Output:

<img width="1028" height="731" alt="output Day5" src="https://github.com/user-attachments/assets/51ffd078-b508-494c-bec0-d4f1c53b8862" />


## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
