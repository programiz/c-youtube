# C Operators
Video Link: [https://youtu.be/_57FcSBtJNU](https://youtu.be/_57FcSBtJNU)
Tutorial Link: [https://www.programiz.com/c-programming/c-operators]()

## Arithmetic Operator
```c
Addition        +
Subtraction     -
Multiplication  *   
Division        /   
Remainder       %   
Increment       ++
Decrement       --
```
## Addition Operators
#### Addition of int variables:
```c
#include <stdio.h>

int main() {

  int x = 12;
  int result = x + 8;
  
  printf("%d", result);
  return 0;
}
```
Another way:
```c
#include <stdio.h>

int main() {

  int x = 12;
  
  printf("%d", x+8);
  return 0;
}

```
**Output**
```
20
```
#### Addition of double variables:
```c
#include <stdio.h>

int main() {

  double x = 12.57;
  double result = x + 8.67;
  
  printf("%.2lf", result);
  return 0;
}
```
**Output**
```
21.24
```
#### Addition of double and int variable:
```c
#include <stdio.h>

int main() {

  double x = 12.57;
  int y = 8;
  double result = x + y;
  
  printf("%.2lf", result);
  return 0;
}
```
**Output**
```
20.57
```

## Division Operator
#### Division with integer numbers:
```c
#include <stdio.h>

int main() {

 int x = 12;
 int result = x / 8;
  
  printf("%d", result); 
  return 0;
}
```

**Output**

```
1
```
#### Division with floating-point numbers:
```c
#include <stdio.h>

int main() {
  double x = 12.00;
  double result = x / 8.00;
  
  printf("%.2lf", result);
  return 0;
}
```
**Output**
```
1.50
```

---
## Remainder Operator

```c
#include <stdio.h>

int main() {

  int x = 12;
  int result = x % 8;
  
  printf("%d", result);
  return 0;
}
```
**Output**
```
4
```
## Increment and decrement Operator
#### Increment Operator
```c
#include <stdio.h>

int main() {

  int x = 12;
  
  printf("%d", ++x);
  return 0;
}
```
**Output**
```c
13
```
#### Decrement Operator
```c
#include <stdio.h>

int main() {

  int x = 12;
  
  printf("%d ", --x);
  return 0;
}
```
**Output**
```c
11
```

## Multiple Operators
```c
#include <stdio.h>

int main() {

  int x = (4 / 2) + (6 * 5) - 1;
  
  printf(" %d", x);
  return 0;
}
```
**Output**
```c
31
```


---
## Programiz Quiz
Q.  What is the value of x in the following code?
```c
int x = 5 + 2 * 9 / 3 - 3;
```
**Options**
1. 18
1. 11
1. 8
1. Error

**Answer: 3**