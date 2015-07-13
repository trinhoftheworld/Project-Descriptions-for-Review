Getting Started with HTML Project Reviewer Guideline
==========================================

## Context

This project is the first project for Introduction to Programming Students. Please keep in mind that these students will come from a background with very little experience programming. At Udacity, our students will learn a lot from getting constructive feedback on their projects.

Since this is the first project they will do, they automatically pass if they submit some HTML code to you. The reviewer’s job is to look over students’ HTML code and critique their HTML code.

Students will be taking notes in HTML from this lesson:

### How does this project fit into the overall program?
Over the course of the program, students will build a web page.  This project is the first stage.

Students are expected to take notes from the mentioned lesson above and will be exposed to basic HTML tags such as `<div>, <h1>, <b>, <em>, <span>`.

The reviewer is expected to read students’ notes and add any clarification or commentary on their notes

The reviewer is also expected to read the students’ HTML code and provide constructive feedback on their code.
Criteria

## Project Description

As long as the student submits some notes in HTML, the project will pass. If the student submitted nothing, please mark the project as “Ungradable” and type in a message to the student outlining why the project is ungradable.

The reviewer should comment and give at least 3 comments on student’ code. One of the comments needs to be a nitpick to help guide students on best practices for HTML coding.

The tone and diction of the comments should be encouraging and supportive. Feedback should be constructive and not insulting or disparaging. It’s very important that these Introduction to Programming students receive a pleasant and helpful experience with their first code review. The encouragement and guidance you will give to these students will set the entire tone throughout their experience in this Nanodegree!

### What should I comment on and expect from students?
We’d like you comment not only on the HTML code, but also the content within the HTML.

* HTML 
  * The html you will see is the first code these students have ever written.  Because of this, it’s especially important that reviews are positive! The feedback you provide them is intended for their learning and they will be continuing to add functionality to their web page through the rest of their Nanodegree program.

You should look for:

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
  * Note that you can leave these comments using the same line-by-line interface for code review comments.

## Watch Outs
Students will first start with using an online tool: www.codepen.io. Most of them will be using the "Export Zip" option in Codepen and will then directly upload this zip onto our servers. Unfortunatley Codepen adds in this extra HTML code at the beginning of their code:

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>CodePen - A Pen by  Mark Nguyen</title>
</head>
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

Please take note that if a student adds in their own header tags such as `<head>` or `<title>` you will probably see double headers due to the extra code CodePen adds. You should let the student know what CodePen does and remind them to check their exported code before the student submits.

