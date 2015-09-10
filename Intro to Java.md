## Project Overview

For this project, students will make a game-playing agent for Connect Four. The code provided to them sets up the GUI and game logic for Connect Four, and the only class they are required to modify is the MyAgent class (they can modify the other classes, but they do not need to).

Please visit [this lesson](https://www.udacity.com/course/viewer#!/c-cs046/l-3064138744/e-3054808770/m-3093088645) from  "Intro to Java Programming" to know more about this project.

## How Grading Works

We have created an [automated tester][1] that does two main things:

1. The tester plays the student's agent against the other agents thousands of times. One of the rubric components specifies that the agent needs to beat these agents a certain number of times, so check for these numbers.
2. The tester also uses checkstyle to check the student's MyAgent class to a small style guide. Double check that naming conventions are followed and that all methods are javadoc documented appropriately (missing class-level javadoc is OK).

To run the tester, [clone the autograder repo][1], paste in the student's MyAgent.java in the src/main/java directory, and run

```
./gradlew
```

(If you're on Windows, you need to use a backslash and run `.\gradlew` instead)

See the tester repo README for more information about grading.  Note that students occasionally change or add files outside of MyAgent.java, and in such cases these files must be included as well to test their project.

[1]: https://github.com/udacity/connect-four-tester

## Review Tips

Here are some tips you'll want to keep in mind when reviewing projects.

### Win percentages (Rubric: Code Functionality)

If a student implements effective `iCanWin` and `theyCanWin` logic and nothing further, their win percentages should be approximately:

* 95+% vs Random Agent
* 80% vs Beginner Agent
* 50% vs Brilliant Agent

If a student's win percentages are significantly lower than that, this is a strong indication that the student has mistakes in their move logic. Be sure to find these: they need to be corrected *even if the student's win percentages still meet specifications.*

### MyAgent should work as both the red and yellow player (Rubric: Code Functionality)

Each agent instance contains an `iAmRed` boolean parameter that indicates whether the agent is playing as red or yellow. As such, the MyAgent code should not assume that it is playing as a particular color. The autograder will test MyAgent as both colors.

### Repetitive code and use of loops (Rubric: Use of Control Flow Statements)

Many students run nested for loops in their win-finding logic to examine each slot on the board. For each slot, there are thirteen configurations around it that could imply a win (four patterns each for horizontal and the two diagonal directions, and one vertical pattern). A student writing 13 `if` statements to check each of these cases in turn is a baseline for passing provided they do so in a neat and organized way.

### Duplicate `iCanWin` and `theyCanWin` implementations (Rubric: Definition and Use of Methods)

You may see projects that have almost identical implementations to determine whether MyAgent can win or the opposing agent can win. To reduce code duplication, projects should be able to create a single method that can be reused for both the same purpose as `iCanWin` and `theyCanWin`.

### Code should follow Java conventions and be fully documented (Rubric: Code Readability)

With the checkstyle linter that's integrated into the automated tester, you can see if the student's code, including MyAgent.java and other student-created classes, adheres to the Java style guide. Checkstyle will help you catch the first two rubric items in the Code Readability section.

Here's an example of checkstyle output. In this case, there are CONSTANTS that weren't declared as `public static final`, and there's a missing `@param` documentation tag for a method.

```
[ant:checkstyle] <path-to-repo>/src/main/java/MyAgent.java:6:27: Name 'BEST_FIELDS' must match pattern '^[a-z][a-zA-Z0-9]*
[ant:checkstyle] <path-to-repo>/src/main/java/MyAgent.java:6:27: Name 'BEST_FIELDS' must match pattern '^[a-z][a-zA-Z0-9]*$'.
[ant:checkstyle] <path-to-repo>/src/main/java/MyAgent.java:7:23: Name 'MAX_TRY' must match pattern '^[a-z][a-zA-Z0-9]*$'.
[ant:checkstyle] <path-to-repo>/src/main/java/MyAgent.java:225:40: Expected @param tag for 'iRed'.
```

**This review may take up to an hour to finish.**
