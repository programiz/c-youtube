# Type Conversion in C Programming
Video Link: [https://youtu.be/xi2wf0Zy2Y4](https://youtu.be/xi2wf0Zy2Y4)
Tutorial Link: [https://www.programiz.com/c-programming]()

### Add two integers

```c
#include <stdio.h>

int main() {

  int a = 5;
  int b = 9;

  int result = a + b;

  printf("%d", result);
  return 0;
}

```
**Output**
```
14
```
### char to int Conversion
```c
#include <stdio.h>

int main() {

  char a = '5';
  int b = 9;

  int result = a + b;

  printf("%d", result);
  return 0;
}

```
**Output**
```
62
```
### double to int Conversion
```c
#include <stdio.h>

int main() {

  double a = 5.67;
  int b = 9;

  int result = a + b;

  printf("%d", result);
  return 0;
}

```
**Output**
```
14
```

### int to double Conversion
```c
#include <stdio.h>

int main() {

  double a = 5.67;
  int b = 9;

  double result = a + b;

  printf("%lf", result);
  return 0;
}

```

**Output**

```
14.670000
```
## Data Type Hierarchy

- long double
- double
- float
- long
- int
- short
- char


---
## Higher data type demoted to lower data type

```c
#include <stdio.h>

int main() {

  int a = 5.67;

  printf("%d", a);
  return 0;
}

```
**Output**
```
5
```
## Explicit Type Conversion

### Convert double data type to int

```c
#include <stdio.h>

int main() {

  double a = 5.67;
  int b = 9;

  double result = (int)a + b;

  printf("%lf", result);
  return 0;
}

```
**Output**
```c
14.000000

```
### Change data type of result variable to int
```c
#include <stdio.h>

int main() {

  double a = 5.67;
  int b = 9;

  int result = (int)a + b;

  printf("%d", result);
  return 0;
}

```
**Output**
```c
14
```

### Change data type of result variable to double

```c
#include <stdio.h>

int main() {

  int a = 9;
  int b = 2;

  double result = a / b;

  printf("%lf", result);
  return 0;
}

```
**Output**
```c
4.000000

```
### Division by converting int to double 

```c
#include <stdio.h>

int main() {

  int a = 9;
  int b = 2;

  double result = (double)a / b;

  printf("%lf", result);
  return 0;
}


```
**Output**
```c
4.500000
```



---
## Programiz Quiz
Q. What is the value of result in the following statement?
```c
int result = '8' + 12;

```
**Options**
1. 20
1. 68
1. Error
1. 12650

**Answer: 2**