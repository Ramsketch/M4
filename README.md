# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() 
{
    int a = 44;
    int b = 3; 
    int result = a << b; 
    printf("Result of %d << %d is %d\n", a, b, result);
    return 0;
}

```

## OUTPUT
<img width="1919" height="1042" alt="Screenshot 2025-10-22 160611" src="https://github.com/user-attachments/assets/db9f98d1-8c9b-4ab9-b41f-ea4d2007f1c8" />










## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() 
{
    int num1, num2;
    scanf("%d", &num1);
    scanf("%d", &num2);
    if(num1 == num2) 
    {
        printf("Both numbers are equal.\n");
    } 
    else 
    {
        printf("Both numbers are not equal.\n");
    }
    return 0;
}

```

## OUTPUT
<img width="1919" height="1033" alt="Screenshot 2025-10-22 160830" src="https://github.com/user-attachments/assets/c3d21a47-53ac-46b4-937e-985d8cfbc24d" />
<img width="1915" height="1034" alt="Screenshot 2025-10-22 160845" src="https://github.com/user-attachments/assets/c0975a04-c6a1-45ed-8396-c3dc48cec68a" />

           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
    char str[100];
    scanf("%[^\n]", str);
    for(int i = 0; str[i] != '\0'; i++)
    {
        if(str[i] >= 'A' && str[i] <= 'Z') 
        {
            str[i] = str[i] + 32; 
        }
    }
    printf("Lowercase : %s\n", str);
    return 0;
}

```

## OUTPUT
<img width="1908" height="1041" alt="Screenshot 2025-10-22 161202" src="https://github.com/user-attachments/assets/47c26a3c-cd10-4009-9da7-f7bbb0f2270b" />





## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() 
{
    char str[100];
    int i = 0,count = 0;
    scanf("%[^\n]", str);
    if(str[0] != '\0') 
    { 
        do
        {
            if(str[i] == ' ' && str[i-1] != ' ' && i != 0)
            {
                count++;
            }
            i++;
        } 
        while(str[i] != '\0');
        count++;
    }
    printf("Total number of words: %d\n", count);
    return 0;
}

```

## OUTPUT
<img width="1919" height="1033" alt="Screenshot 2025-10-22 161501" src="https://github.com/user-attachments/assets/348d4f26-8518-4105-afaf-0afebc59a5d5" />






## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>
int main() 
{
    char c1[100], c2[100];
    int i = 0, flag = 0;
    scanf(" %[^\n]", c1);
    scanf("%s", c2);
    while(c1[i] != '\0' && c2[i] != '\0') 
    {
        if(c1[i] != c2[i]) 
        {
            flag = 1;
            break; 
        }
        i++;
    }
    if(c1[i] != '\0' || c2[i] != '\0')
    {
        flag = 1; 
    }
    if(flag == 0) 
    {
        printf("Strings are same\n");
    } 
    else 
    {
        printf("Strings are not same\n");
    }
    return 0;
}

```


## OUTPUT
<img width="1919" height="1044" alt="Screenshot 2025-10-22 161758" src="https://github.com/user-attachments/assets/518bae84-3d80-4765-862c-3f0c04dff279" />
<img width="1919" height="1040" alt="Screenshot 2025-10-22 161815" src="https://github.com/user-attachments/assets/da2ac474-2db5-47b7-baf8-b056fdc2f867" />


 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

