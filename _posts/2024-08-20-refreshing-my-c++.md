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

#### Learnings:
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

### Part Three: Sample C++ Applications
The goal of this part is to actually build out a few sample C++ applications to prectice what I am learning on the C++ journey.

1. C++ Application: Tic-Tac-Toe
2. C++ Application: Basic Inventory Management System 
3. C++ Application: Personal Expense Tracker


> As always, happy to hear your thoughts... 
{: .prompt-tip }

>
> Modified By: _Martin Thompson_
>
> Last Modified: August 26, 2024-10:38:00