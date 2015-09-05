# Data Analysis with R

## Project evaluation document
Is available from the Description tab inside the Reviews app.

## Sample projects - internal
Please review carefully [these](https://drive.google.com/a/knowlabs.com/folderview?id=0B-ya9aP4zq8ZfkoybDNYYk9GLUlnY2NkWGs5TlNNZ3hlV0pVY1IyYWV4UVBqRjYyWXVkTkE&usp=drive_web) project submissions and their corresponding evaluations. You are going to need a Gmail account to open the folder and add it to your Google Drive (using the button in the top right that says "Add to Drive").  

There are also some very good final projects below (in the *More Udacious Projects* section), that you can share with students.   

## Final Project Instructions (student-facing)
For the final project, you will conduct your own exploratory data analysis and create an RMD file that explores the variables, structure, patterns, oddities, and underlying relationships of a data set of your choice.

The analysis should be almost like a stream-of-consciousness as you ask questions, create visualizations, and explore your data.

This project is open-ended in that we are not looking for one right answer. As John Tukey stated, "The combination of some data and an aching desire for an answer does not ensure that a reasonable answer can be extracted from a given body of data." We want you to ask interesting questions about data and give you a chance to explore. We will provide some options of data sets to explore; however, you may choose to explore an entirely different data set. You should be aware that finding your own data set and cleaning that data set into a form that can be read into R can take considerable time and effort. This can add as much as a day, a week, or even months to your project so only adventure to find and clean a data set if you are truly prepared with programming and data wrangling skills.

### Step One - Choose your Data Set
First, you will choose a data set from the <a href="https://docs.google.com/document/d/1qEcwltBMlRYZT-l699-71TzInWfk4W9q5rTCSvDVMpc/pub" target="_blank">**Data Set Options**</a> document. You should choose a data set based on your prior experiences in programming and working with data. The data set you choose will not increase or decrease your chances of passing the final project. 
In general, <a href="http://vita.had.co.nz/papers/tidy-data.pdf" target="_blank">**tidy data sets**</a> are easier to work with since each variable is a column and each row is an observation; there’s no data cleaning or wrangling involved. We offer guidance below for choosing your data set. Time estimates include reading all of the project instructions and rubric, conducting the analysis, and submitting the final project.

### Step Two - Get Organized
Eventually you’ll want to submit your project (and share it with friends, family, and employers). Get organized before you begin. We recommend creating a single folder on your desktop that will eventually contain:

1. The **RMD file** that contains the analysis, final plots and summary, and reflection (in that order)
2. The **HTML file** that will be knitted from your RMD file
3. The **data set** you used (which you will only submit if you found your own data set)
	
### Step Three - Explore your Data
This is the fun part. Start exploring your data! Keep track of your thoughts as you go (in an RMD file). Please refer to the <a href="https://s3.amazonaws.com/udacity-hosted-downloads/ud651/diamondsExample.html" target="_blank">**Example Project**</a> that we have provided. Your report should look similar! 

### Step Four - Document your Analysis
You will want to document your exploration and analysis in an **RMD file** which you will submit. That file should be formatted in markdown and should contain (in order):

1. **A stream-of-consciousness analysis and exploration of the data.**

    a. Headings and text should organize your thoughts and reflect your analysis as you explored the data.

    b. Plots in this analysis do not need to be polished with labels, units, and titles; these plots are exploratory (quick and dirty). They should, however, be of the appropriate type and effectively convey the information you glean from them.

    c. You can iterate on a plot in the same R chunk, but you don’t need to show every plot iteration in your analysis.

2. **A section at the end called “Final Plots and Summary”**

     You will select three plots from your analysis to polish and share in this section. The three plots should show different trends and should be polished with appropriate labels, units, and titles (see the <a href="https://docs.google.com/document/d/1L2Wwofs6D8Crd0QLZ1-RxBHlVoBZ3mec2xWgxrmUs5I/pub" target="_blank">**Project Rubric**</a> for more information).

3. **A final section called “Reflection”**

    This should contain a few sentences about your struggles, successes, and ideas for future exploration on the data set (see the <a href="https://docs.google.com/document/d/1L2Wwofs6D8Crd0QLZ1-RxBHlVoBZ3mec2xWgxrmUs5I/pub" target="_blank">**Project Rubric**</a> for more information).
    
    
## Project Template File
Please download the <a href="https://s3.amazonaws.com/udacity-hosted-downloads/ud651/projectTemplate.Rmd" target="_blank">**project template file**</a> to get started on your analysis.

## Formatting Notes
We want you to submit a readable RMD file. To help you prepare your project, please look over the following notes.

<ol><li> The knitted HTML output should be readable. Be sure to review your knitted HTML file and check that the code and plots appear correct.</li>
<br>
<li>Comments for R code in a RMD or R-Markdown file are included inside of r blocks by using a hash or pound symbol.</li>
<br>
<pre><code>```{r}
library(ggplot2)
# This is an example of a comment that is not actual code.
```
</code></pre>
<br>
<li>In a RMD or R-Markdown file, use of the hash or pound symbol (#) outside of r blocks of code creates an H1 header.</li>
<h1>This is what an h1 header looks like when it is knitted</h1>
<li>You can use multiple pound symbols to create subsections (h2 tags and so on).</li>
<em>You won't see the hash symbol in front of the text above once you knit the HTML file. See <a href="http://daringfireball.net/projects/markdown/syntax" target="_blank">Markdown Syntax</a> for additional help with Markdown formatting.</em>
<br>
<br>
<li>Check that all your plots can be viewed and that they are sized appropriately for the output, which is the knitted HTML file.</li>
</ol>


## What is included in a submission?

1. The RMD file containing the analysis (final plots and summary, and reflection)
2. the HTML file knitted from the RMD file using the knitr package
3. the original data set and source if you used your own data rather than one recommended by Udacity (Note: do not submit a data set if you used one that Udacity recommended)
4. A list of  Web sites, books, forums, blog posts, github repositories, etc. that you referred to or used in creating your submission (add N/A if you did not use any such resources).

## Example Projects - student facing

Your final project will be an analysis in which you analyze the variables and relationships within a data set. Your **final project** should look similar to this <a href="https://s3.amazonaws.com/udacity-hosted-downloads/ud651/diamondsExample.html" target="_blank">**Example Project**</a>. It should follow the same structure with an **Analysis** section, a **Final Plots** section, and a **Reflection** section. We will provide a template for you to use with these sections already included.

Take at least 10 minutes to review the example project to get a sense of what you will need to do before starting your project.

## More Udacious Projects
These projects go above and beyond the course material, and we hope they serve as inspiration to work with data that interests you and to ask interesting questions.

<a href="https://s3.amazonaws.com/udacity-hosted-downloads/ud651/AtlanticHurricaneTracking.html" target="_blank">Climatology of Atlantic Hurricanes</a> by Dean D. Churchill

<a href="https://s3.amazonaws.com/udacity-hosted-downloads/ud651/GeographyOfAmericanMusic.html" target="_blank">Geography of American Musicians</a> by Stefan Zapf

## Common Problems with Project Submissions - Student Facing

To help you succeed, we recommend comparing your project submission against the following list of common problems. Your project must **avoid** these common problems in order to pass.

* Data processing or transformations (creating a categorical variable) should be included in the RMD file and the final knitted HTML output.

* Reflection section is not included.

* Reflection section is not the last section in the RMD file.

* Final Plots section is not included.

* Final Plots section is not at the end of the RMD file before the Reflection section.

* Final Plots section does not contain three plots.

* One or more plots in the Final Plots section do not reveal a finding or pattern in the data set.

* Final Plots are not polished and are missing titles or units.

* Inappropriate plots are chosen for data in the Final Plots section.

## <a href="https://docs.google.com/document/d/1-f3wM3mJSkoWxDmPjsyRnWvNgM57YUPloucOIl07l4c/pub" target="_blank">Creating Effective Plots</a>

The **Final Plots** section in your RMD file should contain three polished plots that give insight into the data set that you investigated.

**Each plot should also contain a caption or description about what the plot shows.**

In determining whether or not you have three strong plots, please consult the document, **<a href="https://docs.google.com/document/d/1-f3wM3mJSkoWxDmPjsyRnWvNgM57YUPloucOIl07l4c/pub" target="_blank">Creating Effective Plots</a>**. The document covers four common problems that project evaluators have encountered in the past and how those plots can be improved.
