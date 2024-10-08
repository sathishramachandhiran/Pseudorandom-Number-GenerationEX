# Pseudorandom-Number-Generation

## AIM:
 Implementation of Pseudorandom Number Generation Using Standard library

## ALGORITHM:

### 1.Start the program and import the required libraries.
### 2.Seed the random number generator using the current time (i.e) rand(time(0));
### 3.Get the number of random numbers to generate.
### 4.Pass the value for number of iterations and print the numbers.
### 5.End the program.

## PROGRAM:
```C
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/2ec21deb-0fdc-4c7b-ae78-95baf50f9be5)


## RESULT:
The Implementation of Pseudorandom Number Generation Using Standard library is successful.
