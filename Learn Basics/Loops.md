In C++, loops are used to repeatedly execute a block of code as long as a certain condition is true or for a fixed number of iterations. C++ provides three types of loops: `for`, `while`, and `do-while`. Let's explore each of them in detail.

### 1. `for` Loop:

The `for` loop is commonly used when you know in advance how many times you want to iterate.

```cpp
for (initialization; condition; update) {
    // code to be executed
}
```

- **Initialization:** This part is executed once at the beginning and is often used to initialize a loop control variable.
- **Condition:** It is evaluated before each iteration. If it's true, the loop continues; otherwise, it terminates.
- **Update:** Executed at the end of each iteration, usually to update the loop control variable.

Example:

```cpp
#include <iostream>

int main() {
    for (int i = 0; i < 5; ++i) {
        std::cout << i << " ";
    }

    return 0;
}
```

### 2. `while` Loop:

The `while` loop is used when the number of iterations is not known beforehand and is based on a condition.

```cpp
while (condition) {
    // code to be executed
}
```

Example:

```cpp
#include <iostream>

int main() {
    int i = 0;

    while (i < 5) {
        std::cout << i << " ";
        ++i;
    }

    return 0;
}
```

### 3. `do-while` Loop:

The `do-while` loop is similar to the `while` loop, but the condition is checked at the end, so the loop body is executed at least once.

```cpp
do {
    // code to be executed
} while (condition);
```

Example:

```cpp
#include <iostream>

int main() {
    int i = 0;

    do {
        std::cout << i << " ";
        ++i;
    } while (i < 5);

    return 0;
}
```

### Loop Control Statements:

#### `break` Statement:

The `break` statement is used to exit a loop prematurely, before the loop condition becomes false.

```cpp
for (int i = 0; i < 10; ++i) {
    if (i == 5) {
        break; // Exit the loop when i is 5
    }
    std::cout << i << " ";
}
```

#### `continue` Statement:

The `continue` statement is used to skip the rest of the loop body and jump to the next iteration.

```cpp
for (int i = 0; i < 5; ++i) {
    if (i == 2) {
        continue; // Skip the iteration when i is 2
    }
    std::cout << i << " ";
}
```

Loops are fundamental for controlling the flow of a program, and choosing the appropriate loop construct depends on the specific requirements of the task at hand.
