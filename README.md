# C++ Tutorials

#### Setting up C++ on Windows

---

To setup on Windows, you only need to get an Integrated Developer Environment (IDE). In the case of windows, it is best to use [Visual Studio](https://visualstudio.microsoft.com/)  (Not VSCode). 

It takes some time for the download to go through, but all you really want is Desktop Development with C++. If you're learning C++ to use C# in the future, I also recommend geting the .NET Desktop Development as well. 

##### Creating a Project
---

1. Click on File > New Project
2. Visual C++ > General
3. Empty Project
4. Give it a name. For our purposes, we can call it HelloWorld
5. Click Ok, and the project should load. 
   
You will see an area called Solution Explorer (It usually opens on the right side of the sceren). 

1. Right Click on Source Files > Add > New Item
2. For the name, Main.cpp

This will open up Main.cpp. From there, type out or copy and paste:

```C++
#include <iostream>

int main() {
    
    std::cout << "Hello, World!" << std::endl;
    std::cin.get();
}
```

If you right click on your project (The HelloWorld at the top of the tree in Solution Explorer) and click build, it will create your executable. You can run it by going to whatever directory you have your solution stored in inside the Debug folder, and double click helloworld.exe, or you can click Local Windows Debugger at the top of Visual Studio right below the toolbar. 

---

#### Setting up C++ on Mac

Mac and Linux already have a compiler built in to run C++ called clang. You can see this by going into your terminal and typing clang++, g++, gcc, or clang. Since we are just starting with C++, we are going to use Apple's XCode to compile C++ code. 

Go to the App Store and Download XCode. It'll install all the necessary components and the XCode welcome screen should open. 

##### Creating a Project
---

1. Click Create a new XCode Project
2. Choose macOS (at the top) for the template for our project
3. Select Command Line Tool
4. Name it HelloWorld
5. Select C++ as the language.
6. You will need to put in some company. This can be anything com.yourname. It's just some unique identifier
7. Click Next
8. Select the location you want to put things
9. You don't need to let XCode access your Contact

This will build your Project. The settings shown in the beginning aren't really necessary to look at or touch for now.

You should see a main.cpp file already generated upon creation of the project. Go ahead and click on that. 

The code that is in there will also run Hello World, but to keep things consistent, we can type it out. 

```C++
#include <iostream>

int main() {
    
    std::cout << "Hello, World!" << std::endl;
    std::cin.get();
}
```

To build it, just hit the play button. You will have to enable developer mode if you haven't used XCode before. You should see a little terminal pop up down at the bottom and you should see Hello World pop up there.

---

Now that you've got everything set up, let's check out how [C++ works](how.md)
