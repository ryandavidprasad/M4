# EX-16 - Left Shift Operation  
## AIM:  
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int a = 44, b = 3, result;
    result = a << b;
    printf("Result after left shift: %d\n", result);
    return 0;
}
```

## OUTPUT:
```
Result after left shift: 352
```

## RESULT:  
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.


# EX-17 - Two Numbers are Equal or Not  
## AIM:  
Write a C Program to check whether the two numbers are equal or not using simple if statement.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int a, b;
    scanf("%d%d", &a, &b);
    if (a == b) {
        printf("Both numbers are equal\n");
    } else {
        printf("Both numbers are not equal\n");
    }
    return 0;
}
```

## OUTPUT:
```
Input:
5 5
Output:
Both numbers are equal

Input:
4 7
Output:
Both numbers are not equal
```

## RESULT:  
Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully.


# EX-18 - String Lowercase Conversion  
## AIM:  
Write a C Program to convert the given string into lowercase.

## PROGRAM:
```c
#include <stdio.h>
#include <string.h>
#include <ctype.h>
int main() {
    char str[100];
    int i;
    scanf("%[^\n]", str);
    for (i = 0; str[i]; i++) {
        str[i] = tolower(str[i]);
    }
    printf("Lowercase string: %s\n", str);
    return 0;
}
```

## OUTPUT:
```
Input:
HELLO World
Output:
Lowercase string: hello world
```

## RESULT:  
Thus the program to convert the given string into lowercase has been executed successfully.


# EX-19 - Count of Words in a String  
## AIM:  
Write a C Program to count the total number of words in a given string using do while loop.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    char str[100];
    int i = 0, count = 1;
    scanf(" %[^\n]", str);
    do {
        if (str[i] == ' ') {
            count++;
        }
        i++;
    } while (str[i] != '\0');
    printf("Total words: %d\n", count);
    return 0;
}
```

## OUTPUT:
```
Input:
This is a sample string
Output:
Total words: 5
```

## RESULT:  
Thus the program to count the total number of words in a given string using do while loop has been executed successfully.


# EX-20 - Comparing Two Strings Without strcmp()  
## AIM:  
Write a Program to compare two strings without using strcmp().

## PROGRAM:
```c
#include <stdio.h>
int main() {
    char c1[100], c2[100];
    int i = 0, flag = 0;
    scanf("%[^\n]%*c", c1);
    scanf("%s", c2);
    while (c1[i] != '\0' && c2[i] != '\0') {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }
    if (c1[i] != '\0' || c2[i] != '\0') {
        flag = 1;
    }
    if (flag == 0) {
        printf("Strings are same\n");
    } else {
        printf("Strings are not same\n");
    }
    return 0;
}
```

## OUTPUT:
```
Input:
hello
hello
Output:
Strings are same

Input:
hello
world
Output:
Strings are not same
```

## RESULT:  
Thus the C Program to compare two strings without using strcmp() has been executed successfully.
