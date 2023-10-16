**If-Else Statements**

Conditional statements are a fundamental concept in programming that allows you to make decisions based on certain conditions. These statements enable your code to execute different blocks of code depending on whether specific conditions are met or not. In this blog post, we’ll delve into the basics of conditional statements, starting with the ubiquitous if-else statement and gradually exploring more complex scenarios.

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/ffba8bdd-3558-4456-bc0d-8c3053b960f9)

‘if statement’ is used to execute a block of code only if a certain condition is met. It allows us to conditionally execute code based on whether the specified condition is true.

‘else statement’, on the other hand, is an optional companion to the if statement. It specifies what code to execute if the condition in the if statement is not met (i.e. if it is false).

**Let’s break down the flow of control:**

- If the test condition in the if statement is true, a block of code inside the if block will be executed.
- If the test condition is false, the code inside the else block (if present) will be executed.

```
#include<bits/stdc++.h>
using namespace std;

int main() {
int age=10;


if (age >= 18) {
    cout << "You are an adult." << endl;
} else {
    cout << "You are not an adult." << endl;
}

}
```

**Simplifying Code with “else if”**

As your code becomes more complex, you’ll often encounter scenarios where you need to check multiple conditions. Instead of writing multiple independent if statements, you can streamline your code using else if statements.

Let’s say we want to grade students based on their marks within specific ranges:

```
#include <iostream>
using namespace std;

int main() {
    int marks = 54;


    if (marks < 25) {
        cout << "Grade: F" << endl;
    } else if (marks >= 25 && marks <= 44) {
        cout << "Grade: E" << endl;
    } else if (marks >= 45 && marks <= 49) {
        cout << "Grade: D" << endl;
    } else if (marks >= 50 && marks <= 59) {
        cout << "Grade: C" << endl;
    } else if (marks >= 60 && marks <= 69) {
        cout << "Grade: B" << endl;
    } else if (marks >= 70) {
        cout << "Grade: A" << endl;
    } else {
        cout << "Invalid marks entered." << endl;
    }

    return 0;
}

```
**The output will be GRADE C**

- If marks are less than 25, it prints “Grade: F.”
- If marks are between 25 and 44 (inclusive), it prints “Grade: E.”
- If marks are between 45 and 49 (inclusive), it prints “Grade: D.”
- If marks are between 50 and 59 (inclusive), it prints “Grade: C.”
- If marks are between 60 and 69 (inclusive), it prints “Grade: B.”
- If marks are 70 or higher, it prints “Grade: A.”
- If marks are outside the valid range, it prints “Invalid marks entered.”


