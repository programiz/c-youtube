# C Booleans and Comparison Operator
Video Link: [https://youtu.be/TybmJxXRV80](https://youtu.be/TybmJxXRV80)
Tutorial Link: [https://www.programiz.com/c-programming]()

## C Booleans

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value1 = true;
  bool value2 = false;
  
  printf("%d ", value1);
  printf(" %d", value2);

  return 0;
}

```
**Output**
```
1 0
```
## Comparison Operator
```c
>   Greater than
<   Less than
==  Equal to
>=  Greater than or equal to
<=  Less than or equal to
!=  Not equal to
```
## Greater Than Operator
```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (12 > 9);
  
  printf("%d ", value);

  return 0;
}

```
**Output**
```
1
```

### Change value from 12 to 9

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (5 > 9);
  
  printf("%d ", value);

  return 0;
}

```
**Output**
```
0
```

## Less than Operator
```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (5 < 9);
  
  printf("%d ", value);

  return 0;
}

```

**Output**
```
1
```

### Change value from 5 to 9

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (9 < 9);
  
  printf("%d ", value);

  return 0;
}
```

**Output**

```
0
```

## Equal to Operator

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (9 == 9);
  
  printf("%d ", value);

  return 0;
}
```
**Output**

```
1
```
### Change value from 9 to 6

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (9 == 6);
  
  printf("%d ", value);

  return 0;
}

```
**Output**
```
0
```
## Not Equal to Operator

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (9 != 6);
  
  printf("%d ", value);

  return 0;
}
```
**Output**
```
1
```

## Greater Than or Equal To Operator

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (9 >= 6);
  
  printf("%d ", value);

  return 0;
}

```

**Output**
```c
1
```
## Less Than or Equal To Operator

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (9 <= 6);
  
  printf("%d ", value);

  return 0;
}

```
**Output**
```c
0
```

### Comparator operators with floating point numbers
```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  bool value = (9.34 <= 6.87);
  
  printf("%d ", value);

  return 0;
}

```
**Output**
```c
0
```

## Comparison between variables

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  int num1 = 9;
  int num2 = 6;

  bool value = num1 > num2;
  
  printf("%d ", value);

  return 0;
}
```

**Output**
```c
1
```
### Comparison operators with a variable and value
```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  int num1 = 9;

  bool value = num1 > 6;
  
  printf("%d ", value);

  return 0;
}
```

**Output**
```c
1
```
## Logical Operators in C

```c
&&	Logical AND
||	Logical OR
!	Logical Not
```
## AND Operator

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  int age = 18;
  double height = 6.3;
 
  bool result = (age >= 18) && (height > 6.0);
  
  printf("%d ", );

  return 0;
}

```
**Output**
```c
1
```
### Change the value of age to 16

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  int age = 16;
  double height = 6.3;
 
  bool result = (age >= 18) && (height > 6.0);
  
  printf("%d ", );

  return 0;
}

```
**Output**
```c
0
```

## OR Operator

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  int age = 16;
  double height = 6.3;
 
  bool value = (age >= 18) || (height > 6.0);
  
  printf("%d ", value);

  return 0;
}
```
**Output**
```c
1
```

## NOT Operator

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  int age = 16;
 
  bool value = !(age >= 18);
  
  printf("%d ", value);

  return 0;
}
```
**Output**
```c
1
```

### Change the operator >= to <=

```c
#include <stdio.h>
#include <stdbool.h>

int main() {

  int age = 16;
 
  bool value = !(age <= 18);
  
  printf("%d ", value);

  return 0;
}
```
**Output**
```c
0
```

---
## Programiz Quiz
Q. Which of the following code returns false?

**Options:**
1. 9 >= 9
1. 9 > 9
1. 9 <= 9
1. 9 == 9

**Answer: 2**