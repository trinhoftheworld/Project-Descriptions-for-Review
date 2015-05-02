# ![Andy](http://i.imgur.com/fdGeWES.png) What you'll Make

In this stage, you will learn how to use **other people's** code to save you time and effort. This will let you quickly add powerful functionality (like embedded movies) into your page of notes.

Note that you will not be required to submit any of your Python code for this project (though you are welcome to do so). Instead, you will demonstrate your understanding through your HTML notes.

# ![Andy](http://i.imgur.com/fdGeWES.png) Project Specification

By the end of course 3, you will be able to use other people's existing code in your own programming projects. You may choose to use other code by embedding YouTube videos into your own notes web page, but we will not require you to do so.

For this stage, you only have to submit your HTML notes and the corresponding CSS file. Your submission will be evaluated according to the following rubric:

![](http://i.imgur.com/DSfAhUp.png)

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
