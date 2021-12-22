# C Booleans and Comparison Operator
Video Link: [https://youtu.be/K8mntKyBJGc](https://youtu.be/K8mntKyBJGc)
Tutorial Link: [https://www.programiz.com/c-programming/c-if-else-statement]()

## if Statement in C Programming

```c
Syntax :

if (test_condition) {
  // body of if statement
}
```

### Example 1: if Statement
```c
#include <stdio.h>

int main() {
  int age;

  printf("Enter your age: ");
  scanf("%d", &age);

  if (age >= 18) {
    printf("You are eligible to vote");
  }

  return 0;
}
```

**Output**
```
Enter your age: 31
You are eligible to vote
```
### Example 2: if Statement
```c
#include <stdio.h>

int main() {
  int age;

  printf("Enter your age: ");
  scanf("%d", &age);

  if (age >= 18) {
    printf("You are eligible to vote");
  }

  if (age < 18) {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```

**Output**
```
Enter your age: 15
Sorry, you are not eligible to vote
```
## if...else Statement

```c
Syntax: 

if (test_condition) {
  // statements inside if body
}
else {
  // statements inside else body
}
```

### Example : if .. else Statement

```c
#include <stdio.h>

int main() {

  int age = 15;

  if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```

**Output**
```
Sorry, you are not eligible to vote
```

## else if Statement

```c
Syntax: 

if (test_condition1) {
    // statements1
}
else if (test_condition2){
    // statements2
}
else {
    // statements3
}

```
### Example 1: else if statement

```c
#include <stdio.h>

int main() {

  int age = 130;

  if (age > 120) {
    printf("Invalid Age");
  }

  else if (age < 0) {
    printf("Invalid age");
  }

  else if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```

**Output**
```
Invalid Age
```

### Example 2: else if statement

```c
#include <stdio.h>

int main() {

  int age = -4;

  if (age > 120) {
    printf("Invalid Age");
  }

  else if (age < 0) {
    printf("Invalid age");
  }

  else if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```
**Output**

```
Invalid age
```
### Example 3: Using logical operator to combine the conditions

```c
#include <stdio.h>

int main() {

  int age = -1;

  if (age > 120 || age < 0) {
    printf("Invalid Age");
  }

  else if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}

```
**Output**
```
Invalid Age
```
---

## Programming Task

Q. Can you create a program to check whether a number is positive or negative or 0? 

- If number is positive, print "The number is positive"
- If number is negative, print "The number is negative"
- (and) If number is 0, print "The number is 0"

### Solution :
```c
#include <stdio.h>

int main() {

    double number;
    printf("Enter a number: ");
    scanf("%lf", &number);
    
    if (number > 0) {
        printf("The number is positive");
    }
    else if (number < 0) {
        printf("The number is negative");
    }
    else {
        printf("The number is 0");
    }
    
    return 0;
}
``` 
**Output**
```
Enter a number: -8
The number is negative

```
---

## Programiz Quiz
Q. What is the output of the following code?

```c
#include <stdio.h>

int main() {
    
  int a = 5;
  if (!(a % 2 == 0)) {
    printf("Inside If");
  }
  else {
    printf("Inside else");
  }
  return 0;
}
```
**Options:**
1. Inside if
1. Inside else
1. Inside if
   Inside else
1. Error

**Answer: 1**