write a c  programe to enter the age of 50 student and find the student having age in betwwen 15 to 20.

 #include <stdio.h>
#include <conio.h>
int main()
{
    int i, count = 0, age[50];
    
    for (i = 0; i < 5; i++)
    {
        printf("Enter the age of student %d: ", i + 1);
        scanf("%d", &age[i]);
    }
    for (i = 0; i < 5; i++) // Corrected loop condition
    {
        if (age[i] >= 15 && age[i] <= 20)
            count++;
    }
    printf("Number of students between 15 and 20 years old: %d\n", count);
    getch();
    }
