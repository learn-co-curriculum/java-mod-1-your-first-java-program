# Your First Java Program

## Learning Goals

- Create a Java Project in IntelliJ.
- Run your first Java program.
- Explain basic constructs.

## Executing a simple Java program

- Launch IntelliJ Community Edition.
  - When you first open IntelliJ Community Edition after installing it, you will
    see the following screen:

    ![Welcome to IntelliJ ](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/Welcome-to-IntelliJ.png)
- Click "New Project".
  - When you do so, you will be prompted with a window like this:

    ![New Project](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-new-project.png)
  - Let's create a new Java project!
    - Ensure that "New Project" is highlighted in the left-hand sidebar menu.
    - For "Name:" enter in "first-project". This will be the name of your new
      Java project.
    - For "Location:" select the directory you'd like to put your project in.
      This is where the project will live in your computer's file system.
    - Leave "Create Git repository" unchecked. But know that by checking this
      box, it will create a new Git repository for you.
    - Select "Java" for the language.
    - Select "Maven" for the build system. You will learn more about build
      systems a little later on.
    - Select the JDK that you installed in the previous lesson when setting up
      your environment. This should be JDK 11.
  - Click "Create" to create the new Java project. Give IntelliJ a couple of
    minutes to create and load your new project.
- On the left-hand side, you will see the **project view** window. This shows
  the directory structure of the project:

  ![Project View](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-project-view.png)
- Notice that IntelliJ created a `Main.java` file for us under the directory
  `src/main/java/org/example`. Let's open up that file by double-clicking on it
  from the project view!
- When you open it up you should see the following code in the `Main.java` file:

  ![Java Hello World](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-hello-world.png)
- If we want to compile and run this code, we can do so easily from IntelliJ!
  On line 3 or 4 of the code, notice there is a green triangle or play button.
  Click the play button and then choose "Run 'Main.main()'":

  ![Run program](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-run-main.png)
- This will build the code and then execute it! When the program has run,
  you will see a window pop up towards the bottom of IntelliJ. You should see
  that the program printed `Hello world!`
- We could also run the code by pressing the green play button in the
  upper-right hand corner of IntelliJ:

  ![IntelliJ Run](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-play.png)

### Explanation

- An instruction is a command for the computer. In Java, most instructions end
  with a `;`. There are notable exceptions, and we will cover them all in detail
  in upcoming units.
- A method is a grouping of instructions. We use methods to organize instructions
  that belong together.
  - Consider for example that you wanted to explain to someone how to make
    breakfast.
  - You may need to provide that person instructions on how to make toast, how
    to make eggs and how to make a smoothie.
  - Since you still want to be able to say "make me breakfast, please", and have
    that person understand that it means "make toast", "make eggs", and "make a
    smoothie", you would group all those individual instructions in a single
    method.
  - That method might be called `makeBreakfast()`
  - We will cover the exact syntax for a method and for the instructions inside
    that method in a later unit.
- A class is a grouping of methods. In our previous `makeBreakfast()` example,
  we might have a class that represents a chef, and that class may contain the
  instructions to `makeBreakfast()` as well as the instructions to `makeLunch()`
  and `makeDinner()`.
- Java comes with some pre-defined methods that we get to use to access existing
  functionality.
  - For example, Java gives us pre-defined methods to print characters to the
    screen, perform standard math operations, or even send data over a network
    connection.
- Dot notation: access a specific method inside a specific class (we will
  discuss the difference between a class and an object in a later unit).
- Example: `System.out.println()`.
  - `System` is a class that comes with the JDK.
  - `out` is an object in that class.
  - `println` is a method on that object.
  - The `()` allow us to pass information to the method.
- A parameter is information we pass to a method.
- In our example, we are passing the text we want to print on the screen to the
  `println` method.
- Finally, the `;` is how most instructions end in Java.

Put it all together, and you have the following line from our sample class
above:

```java
System.out.println("Hello world!");
```

Note that there are a few more lines of code in our sample class that surround
the instruction above. We will break down what each line means in subsequent
units.

## Install the Java Visualizer Plugin

Now that we have IntelliJ set up a bit more for us, let's install a helpful
plugin called the **Java Visualizer**. The Java visualizer is a tool that can be
used to show what may be happening in the computer's memory when running and
debugging a program. We will install the Java Visualizer into our IntelliJ IDE.

### Action Item

1. In IntelliJ, navigate to File -> Settings or use the keyboard shortcut
   `Ctrl+Alt+S`:

   ![IntelliJ Settings](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-settings.png) 
2. In the "Settings" window, select "Plugins" from the left-hand sidebar menu
   and search for "Java Visualizer":

   ![IntelliJ Plugins](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-plugins.png)
3. Click the green "Install" button next to the plugin to install it.
4. Once installed, at the bottom of the "Settings" window, click "OK".

Now if you open up your `Main.java` and click the little green bug icon next to
the green play button, you can run the program in debug mode.

![IntelliJ Debug](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-debug.png)

When we run in debug mode, a window will again appear towards the bottom of
IntelliJ. But now we should see the Java Visualizer plugin that we installed!

![IntelliJ Java Visualizer](https://curriculum-content.s3.amazonaws.com/java-mod-1/your-first-java-program/intellij-java-visualizer.png)

## Try It Yourself

- Re-create a basic class with a one-line statement to print a message of your
  choosing
- Choose the name of your class and the text you want your class to output

## Conclusion

Great job on running your first program! Over the next few lessons we'll learn
more about how the code is run and basic Java syntax.
