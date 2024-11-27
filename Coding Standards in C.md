## 1. Indentation and Spacing
- **Indentation and Spaces**:
  - Use 4 spaces per indentation level (preferred) or tabs.
  - Avoid mixing spaces and tabs in the same file.
  - Add spaces around operators (`=`, `+`, `-`, etc.)

```c
// Preferred
int main() {
    int a = 10;
    int b = 20;
    int c = a + b;
    printf("Sum of %d and %d is: %d", a, b, c);
    return 0;
}

// Not-preferred
int main() {
    int a=10;
    int b=20;
    int c=a+b;
    printf("Sum of %d and %d is: %d",a+b);
    return 0;
}

```

## 2. Braces Style

- **K&R style (preferred)**:
  - Follow `Kernighan` & `Ritchie` Style
  - Place opening braces `{` on the same line as the statement.
  - Closing braces align with the start of the statement.

```c
// Preferred
int main() {
    if (a > b) {
        printf("a is greater");
    }
}

// Not-preferred (Allman style)
int main()
{
    if (a > b)
    {
        printf("a is greater");
    }
}
```

## 3. Control Flow
  - Add a space between the keyword (`if`, `for`, `while`) and open parentheses.
  - Add a space between close parentheses of control statement and open in-line curly bracket.

```c
// Preferred
#include <stdio.h>
int main() {
    int age;
    scanf("%d", &age);
    if (age > 18) {
        printf("You can vote");
    }
    else {
        printf("You cannot vote");
    }
    return 0;
}

// Not-preferred
#include <stdio.h>
int main(){
    int age;
    scanf("%d", &age);
    if(age > 18){
        printf("You can vote");
    }
    else{
        printf("You cannot vote");
    }
    return 0;
}
```

  - Write semi-colons in a for loop attached to previous statement. And give a space after the semi-colon.
```c
// Preferred
#include <stdio.h>
int main() {
    for (int i = 1; i <= 10; i++) {
        printf("%d ", i);
    }
    return 0;
}

// Not-preferred
#include <stdio.h>
int main() {
    for (int i = 1 ; i <= 10 ; i++) {
        printf("%d ", i);
    }
    return 0;
}

// Not-preferred
#include <stdio.h>
int main() {
    for (int i = 1;i <= 10;i++) {
        printf("%d ", i);
    }
    return 0;
}
```

## Functions
- Don't give a space between the function name and open parentheses, either in function definition or in function calling.
- Add two new lines b/w any two function definitions.
- Separate parameters/arguments with spaces.

```c
// Preferred
#include <stdio.h>
int is_factor(int a, int b) {
    return a % b == 0;
}


int main() {
    // Function call
    int a = 10;
    int b = 2;
    int result = is_factor(a, b);
    printf("%d", result);
    return 0;
}

// Not-preferred
#include <stdio.h>
int is_factor(int a,int b) {
    return a % b == 0;
}
int main() {
    // Function call
    int a = 10;
    int b = 2;
    int result = is_factor(a,b);
    printf("%d", result);
    return 0;
}
```

## Naming Conventions
### Summary Table of Conventions

| Identifier Type       | Convention                  | Example                        |
|-----------------------|-----------------------------|--------------------------------|
| **Variables**         | `lower_snake_case`          | `student_count`, `max_score`  |
| **Functions**         | `lower_snake_case`          | `calculate_area`, `print_sum` |
| **Constants**         | `ALL_CAPS_WITH_UNDERSCORES` | `MAX_SIZE`, `PI`, `MIN_VALUE` |

