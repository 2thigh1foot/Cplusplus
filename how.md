# How it Works

Let's look at the code we wrote to make sure C++ was working. 

```C++
#include <iostream>

int main() { 
    std::cout << "Hello, World!" << std::endl;
    std::cin.get();
}
```

##### Preprocessor Statements

The first thing a compiler does when it receives a file is it preprocesses all of the preprocessor statements. Anything that starts with a `#` is a preprocessor statement. They happen right before the actual compilation. In the case of the `include`, it will find a file (in our case `iostream`) and copy and paste its content into our code automatically. The files that are most commonly included are header files. 

The reason we are including `iostream` is because we need the function `cout` and `cin`. It stands for Input Output Stream. `cout` is Console Output and `cin` is Console Input. 

##### Main Function

This function is very important. Every C++ program needs on as it is the entry point for out application. Our computer will begin executing the code that is inside the main function first, in order. So for the Hello World program, it has the `cout` of Hello World and the `cin.get()`

##### The `<<` operator

This looks like a bitwise shift left, but the left angular brackets are just an overloaded operator. They are functions. In the case of this line:

```C++
std::cout << "Hello, World!" << std::endl;
```

We are pushing the contents of the "Hello, World!" string into `cout` to print the string to the console and then the `std::endl` is pushed onto the end of the "Hello, World!" string to advance the program to the next line. 

The `std::cin.get();` is just waiting for input from the keyboard. 

Even though this program is simple, a lot is happening under the hood!

Let's go ahead and start looking at [variables](variables.md)
