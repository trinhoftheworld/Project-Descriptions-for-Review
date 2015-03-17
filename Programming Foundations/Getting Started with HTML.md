# Reviewer Instructions for Getting Started with HTML
## Who are these students?
These students are enrolled in the Intro to Programming Nanodegree program. They are beginners and brand new to the world of programming. 
## How does this project fit into the overall program?
Over the course of the program, students will build a web page.  This project is the first stage.   

## What should I comment on and expect from students?
We’d like you comment not only on the html, but also the content within the html.

* HTML 
  * The html you will see is the first code these students have ever written.  Because of this, it’s especially important that reviews are positive! The feedback you provide them is intended for their learning and they will be continuing to add functionality to their web page through the rest of their Nanodegree program.
** You should look for:
  * Use of Logical HTML Structure 
    *  All opening tags are closed
  * Use of basic tags such as:
    * \<b>
    * \<em>
    * \<a> with href attribute
    * \<img> with src attribute 
    * \<p>
    * \<span> and \<div> (though they probably won’t know how to use these effectively yet)
    * You should not expect:
      - \<head> or \<body> tags
      - Proper indentation
      - Any CSS or styling
    * For students who meet or exceed expectations at this stage: feel free to introduce a new concept such as \<head> or \<body> tags, proper indentation, etc.. 
* Content within HTML
  * The content of the web page will be notes students have taken on the high level concepts in the first lesson.  As a reviewer, you aren’t expected to check that they have any specific concepts included, but if you see a student has written something that demonstrates any confusion around a specific concept, feel free to clarify it for them. 
Note that you can leave these comments using the same line-by-line interface for code review comments.

##Watch Outs
Students will first start with using an online tool: www.codepen.io. Most of them will be using the "Export Zip" option in Codepen and will then directly upload this zip onto our servers. Unfortunatley Codepen adds in this extra HTML code at the beginning of their code:

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
