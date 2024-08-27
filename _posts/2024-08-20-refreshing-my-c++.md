---
title: Refreshing my C++
description: After many years I am going through and refreshing my C++ skills and bringing them right up to date.
date: 2024-08-20 12:00:00 +0200
categories: [Learning, Languages]
tags: [c++]
---

### Aims:

The primary aims of this are:
1. Refresh the basic concepts of C++
2. Learn from a longer, deeper dive into C++
3. Build out a couple of sample applications in C++

### Part One: Refreshing the Basics [(Mosh Hamedani- C++ for Beginners Tutorial in 1 hour)](https://www.youtube.com/watch?v=ZzaPdXTrSb8&t=442s)
I decided to bring myself a little more up-to-date with this introductory tutorial from Mosh to get set up with a modern C++ development platform before going into a much deeper dive.

#### Notes:
1. I am going to start by provisioning a Windows 11 Hyper-V Virtual Machine for this developer environment.
2. Installation of Visual Studio Code.
3. Build a quick test app - HelloWorld, Done, Success so let's move on.

### Part Two: A Deeper Dive - C++ in One Hour a Day (Sams Teach Yourself)
I had started reading this book about a year ago, and at the time thought that maybe I should look to go through this book in way more detail to get the maximum benefit from its content.

#### LESSON 1 - Getting Started:
1. A Brief History of C++: 
- Initially developed by Bjarne Stroustroup back in 1979, originally to be a successor to C.
- Microsoft Visual Studio 2022 supports C++11, C++14 and C++17.
- C++ is considered an intermediate-level programming language as it allows for both high-level programming of applications as well as low-level programming of libraries that work close to the hardware.
- Applications, operating systems, web services, databases and enterprise software are programmed in C++.
- Software engineers often use C++ as the language of choice for research by physicists and mathematicians - although I believe that languages such as Python are probably in greater use in these areas <- this is my belief.

2. Programming First C++ Application (HelloWorld):
- Create Hello.cpp

```c++
#include <iostream>

int main() {
    std::cout << "Hello Martin, Welcome to the world of C++" << std::endl;
    return 0;
}
```

Exercises
1. Predict code output.

```c++
#include <iostream>

int main() {
    int x = 8;
    int y = 6;
    std::cout << std::endl;
    std::cout << x - y << " " << x * y << " " << x + y;
    std::cout << std::endl;
    return 0;
}
```
Expected output - "2 48 14"
2. Actual output: 2 48 14 [success]
3. What is the error in this program?

```c++
include <iostream>

int main() {
    std::cout << "Hello Buggy World \n";
    return 0;
}
```
4. Corrected program - was missing the "#" for the _include_ directive.

```c++
#include <iostream>

int main() {
    std::cout << "Hello Buggy World \n";
    return 0;
}
```

#### LESSON 2 - The Anatomy of a C++ Program:
##### Notes:
1. #include - Preprocessor Directive 
    1. Runs prior to compilation
    2. Tells the Processor to insert the contents of a file at this point in the file
2. main() body of the program
    1. Execution of a C++ program **always** starts here
    2. It is convention that the function ***main()*** is declared with an **int** return value
    3. Some C++ applications may use a variant of the ***main()*** function like this:
    ```c++
    int main(int argc, char* argv[])
    ```
    4. In this instance **argc** would contain the number of arguments and **argv[]** would be an array of strings containing the actual arguments(?)
3. code that does the actual work in this application
```c++
    std::cout << "Hello Martin, Welcome to the world of C++" << std::endl;
```
4. ***cout*** ("console-out" - pronounced see-out)
    1. ***cout*** is a _stream_ defined by the standard ***std*** _namespace_
    2. In our application we are putting the string literal "_Hello Martin, Welcome to the world of C++_" into this stream by using stream insertion operator ***<<***
5. ***endl*** is used to end a line, akin to inserting a carriage return "\n"
6. In C++ functions need to return a value unless explicitly specified otherwise
    1. ***main*** is a function too, and always returns an integer value
    2. This value is returned back to the operating system (O/S)
    3. It is convention that a value of 0 would indicate success and that a value if -1 would indicate an error has occured
    4. The follwing would be an example of a function that returns no value
```C++
void MyFunction()
```
7. The Concept of Namespaces
    1. Namespaces are names give to parts of code that help in reducing the potential for naming conflict
    2. By using **std::cout** we are telling the compiler to use that one unique **cout** that is provided in the **std** namespace, for example
    ```c++
    #include <iostream>

    int main() {
        using namespace std;

        cout << "Hello Martin, Welcome to the world of C++" << endl;

        return 0;
    }
    ```
8. Functions in C++
    1. Functions enable us to divide the content of the application into functional units that cab be invoked in a sequence of our choosing.
    2. A function, when invoked, typically returns a value to the invoking/calling function.


### Part Three: Sample C++ Applications
The goal of this part is to actually build out a few sample C++ applications to prectice what I am learning on my C++ journey.

1. C++ Application: Tic-Tac-Toe
2. C++ Application: Basic Inventory Management System 
3. C++ Application: Personal Expense Tracker


> As always, happy to hear your thoughts... 
{: .prompt-tip }

>
> Modified By: _Martin Thompson_
>
> Last Modified: August 26, 2024-10:38:00