# ![Andy](http://i.imgur.com/fdGeWES.png) What you'll Make

You will make a computer program using the Python programming language. This program will automatically generates the HTML for your web page. This will allow you to change the HTML structure of any repeated element (for example, a concept or a description) in one place and then automatically regenerate your page.


# ![Andy](http://i.imgur.com/fdGeWES.png) Project Specification

By the time you've gone through the second course, you'll have added a substantial number of new topics to your notes **and** written some code in a new language (Python).

Because of this, you'll submit 3 files.


1. The HTML for your notes.
2. The CSS for your notes.
3. A Python file (saved as `html_generator.py`)

Your project reviewer will review and provide feedback on two aspects of your submission: the Python code you've written and the text content you've added for your notes file.

### 1 - Code Review
Your reviewer will look at the Python code you've written and provide feedback on:

* **Use of Variables**: Your code should take advantage of variables and variable **names** should reflect the **values** they store. 

* **Functions**: Your code should use functions appropriately to avoid repetition. Function parameters should have logical names and should all be used in the body of the function.

* **Appropriate use of Data**: Data types (`strings` vs `lists` for example) should be used appropriately. 

* **Appropriate use of other coding techniques**: Your code should use statements like `if`, `then`, `else`, `while`, etc... appropriately.

### 2 - Content Review
In addition to looking at the code you write, your project reviewer will also read your notes to help ensure you have a good understanding of the most important concepts covered so far. They will be looking for:

* **Understanding of Programming**: Your notes should demonstrate an understanding of what it means to program a computer. 

* **Understanding of Functions**: Your notes should demonstrate an understanding of what functions are and why they are useful.

* **Basic Programming Knowledge**: Your project reviewer won't be looking for anything specific in this area, but will be providing general feedback where appropriate about other programming ideas.

The rubric that will be used is included below:

![](http://i.imgur.com/cUp5mDP.png)
![](http://i.imgur.com/zrbAe13.png)

##Watch Outs
Students may still use an online tool to type up their notes in HTML and CSS: www.codepen.io. Most of them will be using the "Export Zip" option in Codepen and will then directly upload this zip onto our servers. Unfortunately Codepen adds in this extra HTML code at the beginning of their code:

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>CodePen - A Pen by  Mark Nguyen</title>
</head>
```

Most students will have already added this header code into their HTML already and we will see double definitions in their HTML code such as this:

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>CodePen - A Pen by  Mark Nguyen</title>
</head>


<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>My First Project!</title>
</head>
```

Obviously this HTML file fails HTML validation, but for the sake of the student experience, we want you to ignore this when you review their code. You should not fail the student simply because of this extra code that Codepen adds. You should point out out that Codepen adds in this extra information using this sentence:

> It looks you were using CodePen's Zip file exporter! Please be aware that CodePen added this extra code in your HTML file whenever you export your files. This added code would invalidate your HTML code. I suggest you delete this extra code the next time you plan to use CodePen's Zip file exporter.
