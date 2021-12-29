# C Data Types

Video Link: [https://youtu.be/sARaqR0hRI4](https://youtu.be/sARaqR0hRI4)
Tutorial Link: [https://www.programiz.com/c-programming/c-data-types](https://www.programiz.com/c-programming/c-data-types)

## Data Type: int

```c
#include <stdio.h>

int main() {

  int age = 10;
  printf("%d", age);
  
  return 0;
}
```

**Output**

```
10
```

---
## Print variables and values together

```c
#include <stdio.h>

int main() {

  int age = 10;
  printf("Age = %d", number);
  
  return 0;
}
```

**Output**

```
Age = 10
```

---
## Data Type: double and float

```c
#include <stdio.h>

int main() {

  double number = 12.45;
  printf("%lf", number);
  
  return 0;
}
```

**Output**

```
12.450000
```
## Print formatted double output

```c
#include <stdio.h>

int main() {

  double number = 12.45;
  printf("%.2lf", number);
  
  return 0;
}
```

**Output**

```
12.45
```
---
## Print float and double

```c
#include <stdio.h>

int main() {

  double number = 12.45;
  float number1 = 10.9f;

  printf("%.2lf", number);
  printf("\n%f", number1);  

  return 0;
}
```

**Output**

```
12.45
10.900000
```

---
## Print formatted double and float type

```c
#include <stdio.h>

int main() {

  double number = 12.45;
  float number1 = 10.9f;

  printf("%.2lf", number);
  printf("\n%.1f", number1);  

  return 0;
}
```

**Output**

```
12.45
10.9
```

---
## double with exponential number

```c
#include <stdio.h>

int main() {
  
  double number = 5.5e6;
  printf("%lf", number);
  
  return 0;
}
```

**Output**

```
5500000.000000
```

---
## Data Type: char

```c
#include <stdio.h>

int main() {

  char character = 'z';
  printf("%c", character);

  return 0;
}
```

**Output**

```
z
```

---
## Print numeric value of characters

```c
#include <stdio.h>

int main() {

  char character = 'z';
  printf("%c", character);
  printf("  %d", character);

  return 0;
}
```

**Output**

```
z  122
```

---
## sizeof() Data Types

```c
#include <stdio.h>

int main() {

  int age;
  double number;

  printf("int size = %zu", sizeof (age));
  printf("\ndouble size = %zu", sizeof(number));

  return 0;
}
```

**Output**

```
int size = 4
double size = 8
```

---
## Programiz Quiz

Q. What is the output of the following code?

```c
#include <stdio.h>

int main() {
  int a = 5;
  float a = 9.3;
  
  printf("%d", a);
}
```
**Options**
- a. 5
- b. 9.3
- c. 14.3
- d. Error

**Answer d**