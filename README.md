# EX-NO-6-Pseudo-Random-Number

# PAVITHRA S

# 212223220072

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:

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
    return 0;
}

# OUTPUT:
<img width="347" alt="376196570-3d4a60e8-056e-42e1-9639-659e37f1ac81" src="https://github.com/user-attachments/assets/f11d6533-0191-49eb-a68d-418e3bee0d82" />

# RESULT:
The implementation of Pseudorandom Number Generation using Standard library is successful.
