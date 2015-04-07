Students will submit  HTML and CSS files for a web page that only requires the use of basic knowledge of HTML and CSS. 

Here's <a href="http://codepen.io/AndyAtUdacity/full/PwKdry/" target="_blank">one example</a> of what students could make and here is <a href="http://codepen.io/AndyAtUdacity/pen/PwKdry?editors=110" target="_blank">the code</a> that goes along with it.

## Project Specification
Your project reviewer will review and provide feedback on two aspects of your submission: the code you've written and the text you've written about what you've learned.

### 1 - Code Review
Your reviewer will look at the code you've written and provide feedback on:

* **Use of Syntax**: All of your HTML and CSS should be properly formatted and should pass <a href="http://validator.w3.org/#validate_by_input" target="_blank">HTML validation</a> and  <a href="https://jigsaw.w3.org/css-validator/#validate_by_input" target="_blank">CSS validation</a> tests. 

* **Use of Logical HTML Structure**: Content that is logically related should be grouped together within a container element (like a `<div>` or `<span>`). 
* **Use of HTML Classes and CSS Styling**: There shouldn't be any unnecessary repetition in your CSS code. Similar HTML elements should have the same class names.

### 2 - Content Review
In addition to looking at the code you write, your project reviewer will also read your notes to help ensure you have a good understanding of the most important concepts covered so far. They will be looking for:

* **Understanding of Structured Documents**: Your notes should demonstrate an understanding of what it means for computer code to be "structured."
* **The Importance of Avoiding Repetition**: Your notes should contain some explanation of why it's important to avoid repetition when coding.
* **Basic HTML and CSS knowledge**: Your project reviewer won't be looking for anything specific in this area, but will be providing general feedback about these two languages.


##Watch Outs

###Code Pen
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

###HTML validation

If the student does not add a character encoding in the HTML such as `<meta charset="UTF-8">`, your HTML validator might report an error, but on the public website: http://validator.w3.org/, the validator does not throw an error if the character set is missing. To be fair for students, if the only validation error that shows up is the character encoding, do not fail the student and remind the student to add in the character encoding for cross-language compatibility.

