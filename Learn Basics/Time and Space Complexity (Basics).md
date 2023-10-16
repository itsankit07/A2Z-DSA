We are going to discuss the terms time complexity and space complexity. Here, we will learn the basics of them and in the upcoming part, we will learn complex algorithms with a detailed discussion of their time complexity and space complexity.

**What is Time Complexity?**

We can solve a problem using different logic and different codes. Time complexity basically helps to judge different codes and also helps to decide which code is better. In an interview, an interviewer generally judges a code by its time complexity.

Now, the term, time complexity, seems that it is referring to the time taken by a machine to execute a particular code. But in real life, Time complexity does not refer to the time taken by the machine to execute a particular code. 

**Let’s understand why we should not judge any code on the basis of the time taken by a machine.**

If we run the same code in a low-end machine(e.g. old windows machine) and in a high-end machine(e.g. Latest MacBook), we will observe that two different machines take different amounts of time for the same code. The high-end machine will take lesser time as compared to the low-end machine. 

So, the time taken by a machine can be changed depending on the configuration. That is why we should not compare the two different codes on the basis of the time taken by a machine as the time is dependent on it.

**Definition:**

The rate at which the time, required to run a code, changes with respect to the input size, is considered the time complexity. Basically, the time complexity of a particular code depends on the given input size, not on the machine used to run the code.

Let’s understand this using the following diagram:

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/1b2be390-a72a-4a23-9662-57c78bf303ac)


Now, the next question that comes to our mind is how we will represent the time complexity of a code as we are not going to use the standard units like minutes or seconds. Let’s discuss it below:

**How we will represent the time complexity of any code:**

To represent the time complexity, we generally use the Big O notation. The Big O notation looks like the following:

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/2147758d-6b46-414b-ab21-5fb14185a6c9)

Let’s understand this using the following example:

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/a7c1377c-f3a3-4a6c-9c12-8621edee910f)


The time complexity for this code will be nothing but the number of steps, this code will take to be executed. So, if we write this in terms of Big O notation, it will be like O(no. of steps).

Let’s observe the steps for this code:

First, the assigning step(i = 1) will be done.
The second step will be the comparison i.e. i <= 5.
The third step will be the print statement (i.e. cout << “Raj”;).
The fourth step will be the increment(i.e. i++).
In the fifth step, the updated value of i will be again checked i.e. the comparison(i <= 5).
In the sixth step, the print statement will be executed and so on.
This flow will continue until the value of i becomes greater than 5(i.e. 6). In a broader sense, we can observe that the ‘for loop’ will run 5 times and for each time three steps will be surely executed i.e. checking/comparison, printing, and increment. So, the total steps will be 5*3 = 15. And the time complexity in terms of Big O notation will be O(15).

Now, if we write N instead of 5, the number of steps will be then N*3 = 3N and the time complexity will be O(3*N).

But this manual counting process is not feasible for any code. As the ‘for loop’ might run a billion or million times and inside that ‘for loop’, there might be a large no. of operations or some other ‘for loops’ as well. So, we have to find out a better approach to calculate the time complexity of any given code.

Here come the three rules, that we are going to follow while calculating the time complexity:

We will always calculate the time complexity for the worst-case scenario.
We will avoid including the constant terms.
We will also avoid the lower values.
Let’s discuss the rules individually:

-**Calculate the time complexity for the worst-case scenario:**

Before discussing the point we need to understand the three terms i.e. Best Case, Worst Case, and Average Case.

Let’s understand these three terms considering the following piece of code:

![image](https://github.com/itsankit07/A2Z-DSA/assets/91182445/e735cc9c-89d6-4ecf-b9a6-12fe9d9f8785)


**Best Case:** This term refers to the case where the code takes the least amount of time to get executed. For example, if the mark is 10(i.e. < 25), only the first line will be executed and the rest of the lines will be skipped. So, the least amount of steps i.e. only 2 steps are required in this case. This is an example of the best case.
**Worst Case:** This term refers to the case where the code takes the maximum amount of time to get executed. For example, if the mark is 70(i.e. > 65), the last line will be executed after checking all the above conditions. So, the maximum amount of steps i.e. 4 steps are required in this case. This is an example of the worst case.
**Average Case:** This term is pretty self-explanatory. This is basically the case between the best and the worst.
