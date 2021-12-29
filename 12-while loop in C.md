# while loop in C Programming
Video Link: [https://youtu.be/WgS_SF1VrEk](https://youtu.be/WgS_SF1VrEk)
Tutorial Link: [https://www.programiz.com/c-programming/c-do-while-loops]()

### Syntax :

```c
while (condition) {
    // statements inside while
}


```

### Example 1 : infinite while loop
```c
#include <stdio.h>

int main() {

  while (1 < 5) {
    printf("while loop in C \n");
  }

  return 0;
}

```

**Output**
```
while loop in C 
while loop in C 
while loop in C 
while loop in C 
....

```

### Example 2 : while loop
```c
#include <stdio.h>

int main() {

  int count = 1;

  while (count < 5) {
    printf("while loop in C \n");
    printf("Count = %d \n", count);
    count = count + 1;
  }

  return 0;
}

```

**Output**
```
while loop in C 
Count = 1
while loop in C 
Count = 2
while loop in C 
Count = 3
while loop in C 
Count = 4

```
## Create Multiplication Table

```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter the number: ");
  scanf("%d", &number);

  int count = 1;

  while (count <= 10) {
    int product = number * count;
    printf(" %d * %d = %d \n", number, count, product);
    count = count + 1;
  }

  return 0;
}


```
**Output**
```
Enter the number: 8
 8 * 1 = 8 
 8 * 2 = 16 
 8 * 3 = 24 
 8 * 4 = 32 
 8 * 5 = 40 
 8 * 6 = 48 
 8 * 7 = 56 
 8 * 8 = 64 
 8 * 9 = 72 
 8 * 10 = 80 

```

## do...while Loop

**Syntax :**

```c
do {
    // body of loop
} while(condition);
```
### Example 1: do..while
```c
#include <stdio.h>

int main() {

  int count = 1;

  do {
    printf("%d \n", count);
    count = count + 1;
  } while (count < 5);

  return 0;
}


```
**Output**
```
1 
2 
3 
4 

```
### Example 2: do...while loop with false condition
```c
#include <stdio.h>

int main() {

  int count = 5;

  do {
    printf("%d \n", count);
    count = count + 1;
  } while (count < 5);

  return 0;
}

```

**Output**
```
5 
```
---

## Programming Task

Q. Can you use the while loop to print the multiplication table for the given number. Print the number from 10 to 1. So the output would be something like this.

  
  9 * 10 = 90  
  9 * 9 = 81  
  9 * 8 = 72  
  9 * 7 = 63  
  9 * 6 = 54  
  9 * 5 = 45  
  9 * 4 = 36  
  9 * 3 = 27  
  9 * 2 = 18  
  9 * 1 = 9


## Solution :
```c
#include <stdio.h>

int main() {
    int number;
    printf("Enter the number: ");
    scanf("%d", &number);
    
    int count = 10; 
    
    while(count >= 1){
        int product = number * count;
        printf("%d * %d = %d\n", number, count, product);
        count = count - 1;
    }
    return 0;
}
    
```
**Output**
```
Enter the number: 9
9 * 10 = 90
9 * 9 = 81
9 * 8 = 72
9 * 7 = 63
9 * 6 = 54
9 * 5 = 45
9 * 4 = 36
9 * 3 = 27
9 * 2 = 18
9 * 1 = 9
```
---

## Programiz Quiz

Q. Which of the following causes an infinite loop?

**Options:**
1. while (1) {...}  

1. int i = 3;  
   while (i < 4) {...}  

1. int i = 3;  
   do {  
   ...} while(i < 4)  

1. All of the above

**Answer: 4**