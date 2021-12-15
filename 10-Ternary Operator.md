# Ternary Operator in C
Video Link: [https://youtu.be/05xv2nMj6Ls](https://youtu.be/05xv2nMj6Ls)
Tutorial Link: [https://www.programiz.com/c-programming]()

## Syntax :

```c
test_condition ? expression1 : expression2;
```

## Example: Ternary Operator
### Example 1: 
```c
#include <stdio.h>

int main() {

  int age = 15;

  (age >= 18) ? printf("You can vote") : printf("You cannot vote");

  return 0;
}

```

**Output**
```
You cannot vote

```
### Example 2: 
```c
#include <stdio.h>

int main() {

  int age = 24;

  (age >= 18) ? printf("You can vote") : printf("You cannot vote");

  return 0;
}

```

**Output**
```
You can vote
```
## Example 3 : Using variable in ternary operator

```c
#include <stdio.h>

int main() {

  char operator = '+';

  int num1 = 8;
  int num2 = 7;

  int result = (operator == '+') ? (num1 + num2) : (num1 - num2);
  printf("%d", result);

  return 0;
}

```
**Output**
```
15
```

---

## Programming Task

Q. Can you create a program to check whether a number is odd or even? To create this program, create a variable named number and assign a value to it. Then using a ternary operator check if the number variable is odd or even.

- If number is odd, print "The number is Odd"
- If number is even, print "The number is Even"

---

## Programiz Quiz

Q. What is the correct ternary equivalent of the following if...else statement?


```c
if (5 > 3) {
  result = 9;
}
else {
  result = 3;
}
```

**Options:**
1. result = 5 > 3 ? 3 : 5;
1. 5 > 3 ? result = 5 : 3;
1. result = 5 > 3 ? 5 : 3;
1. 5 > 3 ? result = 3 : 5;

**Answer: 3**