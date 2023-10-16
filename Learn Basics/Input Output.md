```
**Including Libraries**

C++ is a versatile language, and it relies on libraries to access various functionalities. To perform tasks like input and output, we include specific libraries at the beginning of our code. For instance, #include<iostream> is used for input and output operations, while #include<math.h> allows us to use mathematical functions. Simply put, libraries provide pre-built functions and tools for us to use in our code.


**The Generic Skeleton**
The generic skeleton of a C++ program consists of two main components: the library inclusion and the main function. After including the necessary libraries, you declare the main function using int main() { /* Your code here */ return 0; }. This serves as the entry point for your program.

#include<iostream>
int main() {
    // Your code here
    return 0;
}```


**Output with cout**
To display output in C++, you’ll commonly use the cout function from the iostream library. However, you need to specify that it belongs to the std (standard) namespace. For instance, std::cout << “Hey, Ankit!”; will print “Hey, Ankit!” to the console. You enclose the text you want to display within double quotation marks.

You can also use std::endl to insert a newline character and flush the output buffer. Here’s the code and its corresponding terminal output:

```#include<iostream>
int main() {
    std::cout << "Hey, 
Ankit!" << std::endl;
    std::cout << "Hey, 
Ankit!";
    return 0;
}```



**using namespace std**

By adding using namespace std; at the beginning of your program, you’re telling the compiler that you want to use all the names from the std namespace without explicitly specifying std:: each time. This can make your code cleaner and more concise.

`#include<iostream>
using namespace std;

int main() {
    cout << "Hey, 
Ankit!" << :endl;
    cout << "Hey, 
Ankit!";
    return 0;
}`

“using namespace std;” is a useful shortcut for simplifying your C++ code, especially when you’re learning the language and writing smaller programs. It helps reduce clutter and makes your code more readable. However, as your programming projects grow in complexity, consider using it sparingly to avoid potential naming conflicts. It’s a tool that can make your C++ journey smoother, so use it wisely.

**Taking User Input using cin**
One of the fundamental aspects of programming is taking input from the user. In C++, this is achieved with the help of the cin stream, which allows you to receive input from the user via the terminal or console.

`#include<iostream>
using namespace std;

int main() {
    int x;
    int y;
    cin >> x >> y;
    cout << "Value of x: " << x << “ and y: “ <<y;
    return 0;
}`

When you run this program, it waits for two separate inputs from the user, which should be entered one after the other, separated by spaces or Enter key presses. Here’s how it works:

- The program waits for the first input (for x).
- You enter a value (e.g., 10) and press Enter.
- cin reads and stores the value in x.
- The program then waits for the second input (for y).
- You enter another value (e.g., 20) and press Enter.
- cin reads and stores this value in y.


**Note:** 

To make the process more convenient, there’s a shortcut that allows you to include almost all standard libraries at once using #include<bits/stdc++.h>.

The bits/stdc++.h header is a shortcut that includes a vast number of standard C++ libraries, making it easier to access a wide range of functions and classes without specifying each library individually. It’s a time-saving approach for programmers, especially when you need several standard libraries in your code.

However, it’s important to be aware of potential compatibility issues and consider the impact on compile time, especially in large projects. When used judiciously, it can be a valuable asset in streamlining your C++ development process.
