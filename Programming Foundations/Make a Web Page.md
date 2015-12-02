Make a Web Page Project Reviewer Guideline
==========================================

## Context

This project is the second project for Introduction to Programming Students. Please keep in mind that these students will come from a background with very little experience programming. At Udacity, our students will learn a lot from getting constructive feedback on their projects.

Students will be taking notes in HTML of the content they have learned in [Stage 1](https://www.udacity.com/course/viewer#!/c-ud000/l-4148129067/m-3646748863)

## Project Description

Students are expected to take notes from the mentioned lesson above and will be exposed to basic HTML tags such as `<div>, <h1>, <p>, <b>, <em>, <span>` and basic CSS rules.

The reviewer is expected to read students’ notes and add any clarification or commentary on their notes, this includes answering any questions the students have.

The reviewer is also expected to read students’ HTML code and provide constructive feedback on their code.

Students will submit HTML and CSS files for a web page that only requires the use of basic knowledge of HTML and CSS. 

Here's <a href="http://codepen.io/AndyAtUdacity/full/PwKdry/" target="_blank">one example</a> of what students could make and here is <a href="http://codepen.io/AndyAtUdacity/pen/PwKdry?editors=110" target="_blank">the code</a> that goes along with it.

## Project Specification

### 1 - Code Review

Reviewers will read the code and provide feedback on:

* **Use of Syntax**: All HTML and CSS should be properly formatted and should pass HTML validation and CSS validation tests.

* **Use of Logical HTML Structure**: Content that is logically related should be grouped together within a container element (like a `<div>` or `<span>`).

* **Use of HTML Classes and CSS Styling**: There shouldn't be any unnecessary repetition in your CSS code. Similar HTML elements should have the same class names.

### 2 - Content Review

Reviewer will also read notes to help ensure students have a good understanding of the most important concepts covered so far. The student must be explicit and specific in their notes. Reviewer should not pass a rubric criteria if the notes are not clear or not detailed enough to demonstrate a student's understanding of:

* **Understanding of Structured Documents**: Notes should demonstrate an understanding of what it means for computer code to be "structured."

  * The student needs to talk about the Document Object Model (DOM) and how the HTML elements can be organized in a “tree-like” structure where one element can contain other elements and how a programmer can traverse the DOM tree to navigate to any element in the DOM.

* **Learning Resources**: Notes include at least 1 link to programming resources (Udacity Forums, Stack Overflow, Mozilla Developer Network for example)


* **Basic HTML and CSS knowledge**: Reviewer won't be looking for anything specific in this area, but will be providing general feedback about these two languages.

The rubric that will be used is included below:

![rubric](http://i.imgur.com/aVLvTOL.png)

## Watch Outs

### CodePen
Students will first start with using an online tool: www.codepen.io. Most of them will be using the "Export Zip" option in CodePen and will then directly upload this zip onto our servers. Unfortunatley CodePen adds in this extra HTML code at the beginning of their code:

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>CodePen - A Pen by  Mark Nguyen</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
```

and this HTML code at the end:

```
</body>
</html>
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

Obviously this HTML file fails HTML validation, but for the sake of delivering a good student experience, we want you to ignore this when you review their code. You should not fail the student simply because of this extra code that CodePen adds. You should point out that CodePen adds in this extra information using this sentence:

> It looks you were using CodePen's Zip file exporter! Please be aware that CodePen added this extra code in your HTML file whenever you export your files. This added code would invalidate your HTML code. I suggest you delete this extra code the next time you plan to use CodePen's Zip file exporter.

### HTML validation

If the student does not add a character encoding in the HTML such as `<meta charset="UTF-8">`, your HTML validator might report an error, but on the public website: http://validator.w3.org/, the validator does not throw an error if the character set is missing. To be fair for students, if the only validation error that shows up is the character encoding, do not fail the student and remind the student to add in the character encoding for cross-language compatibility.
