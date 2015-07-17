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

See the tester repo README for more information about grading.

[1]: https://github.com/udacity/connect-four-tester


**This review may take up to an hour to finish.**
