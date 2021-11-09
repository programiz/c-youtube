# Take Input in C
Video Link: [https://youtu.be/L2H2rtCLB-0](https://youtu.be/L2H2rtCLB-0)
Tutorial Link: [https://www.programiz.com/c-programming]()

## Comments in C
```c
#include <stdio.h>

int main() {

  // create a variable
  int data = 34;

  // print the value of data variable
  printf("Data = %d", data);

  return 0;
}

```

**Output**

```
Data = 34
```


#### Comment and code can be on the same line like this


```c
#include <stdio.h>

int main() {

  int data = 34;    // create a variable

  printf("Data = %d", data);   // print the variable

  return 0;
}

```

**Output**

```
Data = 34

```

---
## Prevent Executing Code Using Comments

```c
#include <stdio.h>

int main() {
    
  int age;
  double height;
  
  printf("Enter the age: ");
  scanf("%d", &age);
  
  printf("Enter the height: ");
  scanf("%lf", &height);
  
  printf("Age = %d", age);
  printf("\nHeight = %.1lf", height);

  return 0;
}

```

**Suppose, height input is not required so we will comment it out**

```c
#include <stdio.h>

int main() {
    
  int age;
  // double height;
  
  printf("Enter the age: ");
  scanf("%d", &age);
  
  // printf("Enter the height: ");
  // scanf("%lf", &height);
  
  printf("Age = %d", age);
  // printf("\nHeight = %.1lf", height);

  return 0;
}

```
**Output**

```
Enter the age: 29
Age = 29

```
---
## Multiline Comments in C Programming

```c
This program takes age input from the user
It stores it in the age variable
And, print the value using printf()

#include <stdio.h>

int main() {
    
  int age;
  
  printf("Enter the age: ");
  scanf("%d", &age);
 
  printf("Age = %d", age);

  return 0;
}

```

**Multiline commenting above program**


```
/* This program takes age input from the user
It stores it in the age variable
And, print the value using printf() */

#include <stdio.h>

int main() {
    
  int age;
  
  printf("Enter the age: ");
  scanf("%d", &age);
 
  printf("Age = %d", age);

  return 0;
}

```
**Output**

```
Enter the age: 29
Age = 29

```
## Keyboard Shortcut
### Cmd + shift + / for multiline comments

```
/* This program takes age input from the user
It stores it in the age variable
And, print the value using printf() */

#include <stdio.h>

int main() {
    
  int age;
  
  printf("Enter the age: ");
  scanf("%d", &age);
 
  printf("Age = %d", age);

  return 0;
}

```
###  Cmd + / for singleline comment

```c
// This program takes age input from the user
// It stores it in the age variable
// And, print the value using printf()

#include <stdio.h>

int main() {
    
  int age;
  
  printf("Enter the age: ");
  scanf("%d", &age);
 
  printf("Age = %d", age);

  return 0;
}

```

---
## Programiz Quiz
Q.  What is the correct way to comment in C programming?

**Options**
1. //
2. #
3. <!--->
4. All of the above

**Answer: 1**