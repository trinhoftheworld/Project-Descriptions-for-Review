Allow Comments Reviewer Guideline
==========================================

## Context

This project involves using Google App Engine to host a webserver using Python. Students go through a portion of the Udacity Class [Web Development](https://www.udacity.com/course/web-development--cs253).

Here is the actual link to the Stage 4 videos that students go through in the Intro to Programming Nanodegree: [Stage 4](https://www.udacity.com/course/viewer#!/c-ud000/l-4190509137/m-3630598767)

The reviewer should have knowledge of Python and Web Development in Python. The framework that students apply is `webapp2` for WSGI and `jinja2` for the templating engine. The reviewer should quickly review Stage 4 to get familiar with Webapp2 and Jinja2 to get ready to review this project.

## Project Description
The reviewer is expected to read students’ notes and add any clarification or commentary on their notes. The reviewer is also expected to provide constructive feedback on students’ Python code and HTML template files. Ideally the reviewer should give some tips on style according to the [Udacity Style Guide](http://udacity.github.io/frontend-nanodegree-styleguide/), but this is not required.

The student will submit their entire GAE webapp contents which should at minimum include:

* A Python file
* A YAML file
* An HTML template file

## 1 - Web Page / Code Review

The reviewer will be looking for some basic functionality in your web page.
Namely, the page should:

* Be hosted on Google App Engine
* Allow users to add content to your site by submitting a form (with or without
  signing in)
* Use HTML escaping so that when users enter text like this: "*`<b>` tags are
  used to make text bold*" it displays properly.
* Properly save content so that when a user adds text and then refreshes the
  page it still displays the newly-added content

The reviewer will also look at the code. They will be looking for:

* Proper use of GET and POST requests
* Use of separate HTML files / templates where appropriate (no HTML longer than
  5 lines should be written in your Python file(s))
* Reasonable code readability:
  * No unused code
  * No commented out code
  * Informative variable / function / class names
  * No "magic numbers" (a magic number is a number that is used in the code
    without explanation. In these situations you should assign that number to a
    variable with a logical name)
* Python is used for validating user input. It is not enough to use client-side validations such as form validations because not all browsers support proper form validations (ex: Safari). Furthermore, a hacker can bypass form validations by accessing a browser's Development Tools. At a minimum if a user inputs a blank input and an error is raised, this section should pass.

## 2 - Content Review

The reviewer will also read the text content on your page which
pertains to course 4. They will be looking for notes which demonstrate an
understanding of:

 **Servers**: Students' notes should elaborate on:
* How POST and GET requests are processed by the server differently
* How the server responds to these GET and POST requests

**The Importance of Validating Input**: Students' notes should elaborate on:
* Why validating user input is important in terms of site security as well as user experience
* What is a possible consequence of failing to validate user input

**HTML Templates and Abstraction**: Students' notes should elaborate on:
* Why programmers use HTML templates
* How these templates allow programmers to avoid repetition
* Why avoiding repetition (specifically with HTML templates) is important regards to reducing time spent coding and reducing time spent debugging 

The rubric that will be used is included below:

![Rubric, Pt. 1](http://i.imgur.com/zsHe9mw.png)
![Rubric, Pt. 2](http://i.imgur.com/Zf5yr3o.png)

## Watch Outs
Students may still use an online tool to type up their notes in HTML and CSS: www.codepen.io. Most of them will be using the "Export Zip" option in CodePen and will then directly upload this zip onto our servers. Unfortunatley CodePen adds in this extra HTML code at the beginning of their code:

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

Obviously this HTML file fails HTML validation, but for the sake of the student experience, we want you to ignore this when you review their code. You should not fail the student simply because of this extra code that CodePen adds. You should point out out that CodePen adds in this extra information using this sentence:

> It looks you were using CodePen's Zip file exporter! Please be aware that CodePen added this extra code in your HTML file whenever you export your files. This added code would invalidate your HTML code. I suggest you delete this extra code the next time you plan to use CodePen's Zip file exporter.
