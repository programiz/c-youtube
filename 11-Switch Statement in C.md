# Switch Statement in C Programming
Video Link: [https://youtu.be/u6mb8NNwojA](https://youtu.be/u6mb8NNwojA)
Tutorial Link: [https://www.programiz.com/c-programming/c-switch-case-statement](https://www.programiz.com/c-programming/c-switch-case-statement)

### Syntax :

```c
switch(variable/expression) {
    case value1:  
        // body of case 1
        break;

    case value2:  
        // body of case 2
        break;

    case valueN:
        // body of case N
        break;

    default:
        // body of default
}

```

### Example 1 : print the day of a week
```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter a number between 1 to 7: ");
  scanf("%d", &number);

  switch(number) {
    case 1:
      printf("Sunday");
      break;

    case 2:
      printf("Monday");
      break;

    case 3:
      printf("Tuesday");
      break;

    case 4:
      printf("Wednesday");
      break;

    case 5:
      printf("Thursday");
      break;

    case 6:
      printf("Friday");
      break;

    case 7:
      printf("Saturday");
      break;

    default:
      printf("Invalid Number");
  }

return 0;
}

```

**Output**
```
Enter a number between 1 to 7: 5
Thursday

```
### Example 2 : Removing break statement from previous example
```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter a number between 1 to 7: ");
  scanf("%d", &number);

  switch(number) {
    case 1:
      printf("Sunday ");

    case 2:
      printf("Monday ");

    case 3:
      printf("Tuesday ");

    case 4:
      printf("Wednesday ");

    case 5:
      printf("Thursday ");

    case 6:
      printf("Friday ");

    case 7:
      printf("Saturday ");

    default:
      printf("Invalid Number");
  }

return 0;
}

```

**Output**
```
Enter a number between 1 to 7: 5
Thursday Friday Saturday Invalid Number

```
## switch with multiple case

```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter a number between 1 to 7: ");
  scanf("%d", &number);

  switch(number) {
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      printf("Weekday");
      break;
      
    case 1:
    case 7:
      printf("Weekend");
      break;

    default:
      printf("Invalid Number");
  }

return 0;
}

```
**Output**
```
Enter a number between 1 to 7: 4
Weekday

```

## Simple Calculator

```c
#include <stdio.h>

int main() {

  char operator;
  printf("Choose an operator ['+', '-', '*', '/']: ");
  scanf("%c", &operator);
  
  double num1, num2;
  
  printf("Enter first number: ");
  scanf("%lf", &num1);
  
  printf("Enter second number: ");
  scanf("%lf", &num2);
  
  double result;

  switch(operator) {
    case '+':
      result = num1 + num2;
      break;
    case '-':
      result = num1 - num2;
      break;
    case '/':
      result = num1 / num2;
      break;
    case '*':
      result = num1 * num2;
      break;

    default:
      printf("Invalid Operator");
  }
  
  printf("%.2lf", result);

return 0;
}

```
**Output**
```
Choose an operator ['+', '-', '*', '/']: +
Enter first number: 8
Enter second number: 12
20.00

```
---

## Programming Task

Q. Use the switch statement to create a program that will find the month based on the number input. Here, take the input number from 1 to 12. And, print the corresponding month based on the input value.

- If number is 1, print January
- If number is 2, print February
- If number is 3, print March, and so on.

## Solution :
```c
#include <stdio.h>

int main() {
    
    int number;
    printf("Enter a number of a month between 1 to 12: ");
    scanf("%d", &number);
    
    switch (number) {
        case 1:
            printf("January");
            break;
        case 2:
            printf("February");
            break;
        case 3:
            printf("March");
            break;
        case 4:
            printf("April");
            break;
        case 5:
            printf("May");
            break;
        case 6:
            printf("June");
            break;
        case 7:
            printf("July");
            break;
        case 8:
            printf("August");
            break;
        case 9:
            printf("September");
            break;
        case 10:
            printf("October");
            break;
        case 11:
            printf("November");
            break;
        case 12:
            printf("December");
            break;
        default:
            printf("Enter number between 1 to 12 only");
    }
    
    return 0;
}
```

**Output**
```
Enter a number of a month between 1 to 12: 44
Enter number between 1 to 12 only
```
---

## Programiz Quiz

Q. Which of the cases is executed in the following code?

```c
int number = 4;

switch(number) {
  case 1:
  case 2:
  default:
}

```

**Options:**
1. case 1
1. case 2
1. case 4
1. default

**Answer: 4**