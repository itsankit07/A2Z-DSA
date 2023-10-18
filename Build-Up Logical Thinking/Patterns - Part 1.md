**Pattern-1: Rectangular Star Pattern**

Problem Statement: Given an integer N, print the following pattern.

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/dc44f079-e255-41c5-a724-bd91b5710851)

**Examples -**

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/58bb24cc-13ca-4b81-9a3a-27c7c44dc280)

**Approach:**

There are 4 general rules for solving a pattern-based question: 

- We always use nested loops for printing the patterns. For the outer loop, we count the number of lines/rows and loop for them.
- Next, for the inner loop, we focus on the number of columns and somehow connect them to the rows by forming a logic such that for each row we get the required number of columns to 
  be printed.
- We print the ‘*’ inside the inner loop.
- Observe symmetry in the pattern or check if a pattern is a combination of two or more similar patterns.

In this particular problem, we run the outer loop for N times since we have N rows to be printed, the inner loop also runs for N times as we have to print N stars in each row. This way we get a rectangular star pattern (square) with an equal number of rows and columns.

```
#include <bits/stdc++.h>
using namespace std;

void pattern1(int N)
{
    // This is the outer loop which will loop for the rows.
    for (int i = 0; i < N; i++)
    {
        // This is the inner loop which here, loops for the columns
        // as we have to print a rectangular pattern.
        for (int j = 0; j < N; j++)
        {
            cout << "* ";
        }
       
        // As soon as N stars are printed, we move to the
        // next row and give a line break otherwise all stars
        // would get printed in 1 line.
        cout << endl;
    }
}

int main()
{   
    // Here, we have taken the value of N as 5.
    // We can also take input from the user.
    int N = 5;

    pattern1(N);

    return 0;
}
```


**Output**

```
* * * * *
* * * * *
* * * * *
* * * * *
* * * * *
```

----------------------------------------------------------------------------------------------------------------------------

**Pattern-2: Right-Angled Triangle Pattern**

Problem Statement: Given an integer N, print the following pattern : 

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/ec5ffa54-c4e7-413f-ad83-2fbad2817573)

**Examples:**

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/e95f26d1-e8fc-4972-b402-375827267ce4)

**Solution**

In this problem, we run the outer loop for N times as we have to print N rows, and since we have to print a right-angled triangle/pyramid which must be upright, the inner loop will run for the row number in each iteration. For eg: 1 star for row 1, 5 stars for row 5, and so on.

**Code**

```
#include <bits/stdc++.h>
using namespace std;

void pattern2(int N)
{
    // This is the outer loop which will loop for the rows.
    for (int i = 0; i < N; i++)
    {
        // This is the inner loop which loops for the columns
       // no. of columns = row number for each line here.
        for (int j = 0; j <=i; j++)
        {
            cout << "* ";
        }
       
        // As soon as stars for each iteration are printed, we move to the
        // next row and give a line break otherwise all stars
        // would get printed in 1 line.
        cout << endl;
    }
}

int main()
{   
    // Here, we have taken the value of N as 5.
    // We can also take input from the user.
    int N = 5;

    pattern2(N);

    return 0;
}
```
**OUTPUT**
```
* 
* * 
* * * 
* * * * 
* * * * *

```
----------------------------------------------------------------------------------------------------------------------------
**Pattern – 3: Right-Angled Number Pyramid**

Problem Statement: Given an integer N, print the following pattern : 

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/144bcdaf-3b4c-4e55-8bd1-bf698560d074)

**Examples**

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/9b094196-052a-4f42-8d46-c9a34b2c17f0)

**Solution**

In this pattern, we run the outer loop for N times as we have to print N rows, and since we have to print a right-angled triangle/pyramid which must be upright, so the inner loop will run for the row number in each iteration. For eg: 1 number for row 1, 5 numbers for row 5, and so on. The only difference between this pattern and pattern 2 is that here we print numbers looping from 1 to the row number for each row instead of printing stars.

**CODE**

```
#include <bits/stdc++.h>
using namespace std;

void pattern3(int N)
{
    // This is the outer loop which will loop for the rows.
    for (int i = 1; i <= N; i++)
    {
        // This is the inner loop which loops for the columns
       // no. of columns = row number for each line here.
       // Here, we print numbers from 1 to the row number
       // instead of stars in each row.
        for (int j = 1; j <=i; j++)
        {
            cout <<j<<" ";
        }
       
        // As soon as numbers for each iteration are printed, we move to the
        // next row and give a line break otherwise all numbers
        // would get printed in 1 line.
        cout << endl;
    }
}

int main()
{   
    // Here, we have taken the value of N as 5.
    // We can also take input from the user.
    int N = 5;

    pattern3(N);

    return 0;
}
```
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```






