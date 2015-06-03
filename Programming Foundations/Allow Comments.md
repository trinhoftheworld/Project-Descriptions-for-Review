# ![Andy](http://i.imgur.com/fdGeWES.png) Project Specification

This project involves using Google App Engine to host a webserver using Python. Students go through a portion of the Udacity Class [Web Development](https://www.udacity.com/course/web-development--cs253).

Here is the actual link to the Stage 4 videos that students go through in the Intro to Programming Nanodegree: [Stage 4](https://www.udacity.com/course/viewer#!/c-ud000/l-4190509137/m-3630598767)

The reviewer should have knowledge of Python and Web Development in Python. The framework that students apply is `webapp2` for WSGI and `jinja2` for the templating engine. The reviewer should quickly review Stage 4 to get familiar with webapp2 and jinja2 to get ready to review this project.

## 1 - Web Page / Code Review

Your reviewer will be looking for some basic functionality in your web page.
Namely, your page should:

* Be hosted on Google App Engine
* Allow users to add content to your site by submitting a form (with or without
  signing in, that's up to you).
* Use HTML escaping so that when users enter text like this: "*`<b>` tags are
  used to make text bold*" it displays properly.
* Properly save content so that when a user adds text and then refreshes the
  page it still displays the newly-added content.

Your reviewer will also look at your code. They will be looking for:

* Proper use of GET and POST requests.
* Use of separate HTML files / templates where appropriate (no HTML longer than
  5 lines should be written in your Python file(s)).
* Reasonable code readability:
  * No unused code
  * No commented out code
  * Informative variable / function / class names.
  * No "magic numbers" (a magic number is a number that is used in the code
    without explanation. In these situations you should assign that number to a
    variable with a logical name).

## 2 - Content Review

Your project reviewer will also read the text content on your page which
pertains to course 4. They will be looking for notes which demonstrate an
understanding of:

**Servers**: Your notes should demonstrate a basic understanding of how servers
handle requests, process them, and deliver responses.

**The Importance of Validating Input**: Your notes should acknowledge the
importance of validating user input, especially the implications that
validation has on site security and user experience.

**HTML Templates and Abstraction**: Your notes should show an understanding of
why programmers use HTML templates, how these templates allow programmers to
avoid repetition, and understanding of **why** avoiding repetition is
important.

The rubric that will be used is included below:

![Rubric, Pt. 1](http://i.imgur.com/zsHe9mw.png)
![Rubric, Pt. 2](http://i.imgur.com/Zf5yr3o.png)

##Watch Outs
Students may still use an online tool to type up their notes in HTML and CSS: www.codepen.io. Most of them will be using the "Export Zip" option in Codepen and will then directly upload this zip onto our servers. Unfortunatley Codepen adds in this extra HTML code at the beginning of their code:

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
