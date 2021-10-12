# C Variables

Video Link: [https://youtu.be/h4VBpylsjJc](https://youtu.be/h4VBpylsjJc)
Tutorial Link: [https://www.programiz.com/c-programming/c-variables-constants]()


## Print Line of Text

```c
#include <stdio.h>

int main() {

  int age = 25;
  printf("C Programming");

  return 0;
}
```

**Output**

```
C Programming
```

---
## Print Variable

```c
#include <stdio.h>

int main() {

  int age = 25;
  printf("%d", age);

  return 0;
}
```

**Output**

```
25
```

---
## Print Text and Variable Together

```c
#include <stdio.h>

int main() {
  
  int age = 25;
  printf("Age: %d", age);

  return 0;
}
```

**Output**

```
Age: 25
```

---
## Change Value of Variable

```c
#include <stdio.h>

int main() {

  int age = 25;
  printf("Age: %d ", age);

  age = 31;
  printf("New age:  %d", age);

  return 0;
}
```

**Output**

```
Age: 25 New age: 31
```

---
## Change Value of Variable Example 2

```c
#include <stdio.h>

int main() {

  int age = 25;
  printf("Age: %d", age);

  age = 31;
  printf("\nNew age value: %d", age);

  return 0;
}
```

**Output**

```
Age: 25
New age value: 31
```

---
## Assign one variable to another variale

```c
#include <stdio.h>

int main() {

  int firstNumber = 33;
  printf("first Number = %d ", firstNumber);

  int secondNumber = firstNumber;
  printf("\nsecond Number = %d", secondNumber);

  return 0;
}
```

**Output**

```
first Number = 33
second Number = 33
```

## Declare Multiple Variables at once

```c
#include <stdio.h>

int main() {
    int variable1, variable2; 
    return 0;
}
```

```c
#include <stdio.h>

int main() {
    int variable1, variable2 = 25; 
    return 0;
}
```

---
## Programiz Quiz

**Q. Can you guess the output of this program?**

```c
#include <stdio.h>

int main() {

  int number1 = 33;
  printf("%d ", number1);
  printf("%d", number2);

  return 0;
}
```

**Options**
a. 33
b. 3333
c. 33 33
d. '33.0'


**Correct Answer: c** 