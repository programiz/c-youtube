# C Struct
Video Link: [https://youtu.be/gt9YPl6O9ZM](https://youtu.be/gt9YPl6O9ZM)  
Tutorial Link: [https://www.programiz.com/c-programming/c-structures](https://www.programiz.com/c-programming/c-structures)
 
## C Struct

```c
#include <stdio.h>

struct Person {
  double salary;
  int age;
};

int main() {

  struct Person person1;

  person1.age = 25;
  person1.salary = 4321.78;
  printf("Age of person1: %d\n", person1.age);
  printf("Salary of person1: %.2lf", person1.salary);
  
  return 0;
}

```
**Output**
```
Age of person1: 25
Salary of person1: 4321.78

```
**Create the struct variable and initialize members in the same line**
```c
#include <stdio.h>

struct Person {
  double salary;
  int age;
};

int main() {

  struct Person person1 = {.age = 25, .salary = 4321.78};
  struct Person person2 = {.age = 31, .salary = 78943.2};

  printf("Age of person1: %d\n", person1.age);
  printf("Salary of person1: %.2lf", person1.salary);

  printf("\nAge of person2: %d\n", person2.age);
  printf("Salary of person2: %.2lf", person2.salary); 
  
  return 0;
}

```
**Output**
```
Age of person1: 25
Salary of person1: 4321.78
Age of person2: 31
Salary of person2: 78943.20
```
## typedef in Struct

```c
#include <stdio.h>

typedef struct Person {
  double salary;
  int age;
} person;

int main() {

  person person1;

  person1.age = 25;
  person1.salary = 4321.78;
  printf("Age of person1: %d\n", person1.age);
  printf("Salary of person1: %.2lf", person1.salary);
  
  return 0;
}

```
**Output**
```
Age of person1: 25
Salary of person1: 4321.78

```
## Sum of Complex Numbers

```c
#include <stdio.h>

typedef struct Complex {
  double real;
  double imag;
} complex;

int main() {

  complex c1 = {.real = 21.87, .imagine = 30};
  complex c2 = {.real = 13.34, .imagine = 112.23};

  complex sum;

  sum.real = c1.real + c2.real;
  sum.imagine = c1.imagine + c2.imagine;

  printf("Result is %.2lf + %.2lfi", sum.real, sum.imagine);

  return 0;
}

```
**Output**
```
Result is 35.21 + 142.23i
```
---

## Programming Task
Create a program to find the differences between three complex numbers.

Perform the subtraction between complex numbers by subtracting the real part of one complex number from other complex numbers and same for the imaginary part too.

**Solution**
```c
#include <stdio.h>

typedef struct Complex {
    double real;
    double imagine;
} complex;

int main() {
    
    complex c1 = {.real = 28.24, .imagine = 40};
    complex c2 = {.real = 36.3, .imagine = 19.1};
    complex subtract;
    
    subtract.real = c1.real - c2.real;
    subtract.imagine = c1.imagine - c2.imagine;
    
    printf("Result is %.2lf + %.2lfi", subtract.real, subtract.imagine);
    
    return 0;
}
```

**Output**
```
Result is -8.06 + 20.90i
```
---
 
## Programiz Quiz
 
Q. What is the name of the variable of the following struct?  

struct Test {  
    double testScore;  
    int testCount;  
} firstTest;


**Options:**
1. testScore
1. struct
1. firstTest
1. Test

**Answer: 3**


