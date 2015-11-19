## Building a Student Intervention System

As education has grown to rely more and more on technology, more and more data is available for examination and prediction. Logs of student activities, grades, interactions with teachers and fellow students, and more are now captured through learning management systems like Canvas and Edmodo and available in real time. This is especially true for online classrooms, which are becoming more and more popular even at the middle and high school levels.

Within all levels of education, there exists a push to help increase the likelihood of student success without watering down the education or engaging in behaviors that raise the likelihood of passing metrics without improving the actual underlying learning. Graduation rates are often the criteria of choice for this, and educators and administrators are after new ways to predict success and failure early enough to stage effective interventions, as well as to identify the effectiveness of different interventions.

Toward that end, your goal as a software engineer hired by the local school district is to model the factors that predict how likely a student is to pass their high school final exam. The school district has a goal to reach a 95% graduation rate by the end of the decade by identifying students who need intervention before they drop out of school.
You being a clever engineer decide to implement a student intervention system using concepts you learned from supervised machine learning. Instead of buying expensive servers or implementing new data models from the ground up, you reach out to a 3rd party company who can provide you the necessary software libraries and servers to run your software.

However, with limited resources and budgets, the board of supervisors wants you to find the most effective model with the least amount of computation costs (you pay the company by the memory and CPU time you use on their servers).
In order to build the intervention software, you first will need to analyze the dataset on students’ performance. Your goal is to choose and develop a model that will predict the likelihood that a given student will pass, thus helping diagnose whether or not an intervention is necessary. Your model must be developed based on a subset of the data that we provide to you, and it will be tested against a subset of the data that is kept hidden from the learning algorithm, in order to test the model’s effectiveness on data outside the training set.

**Your model will be evaluated on three factors:**

- Its <a href="https://en.wikipedia.org/wiki/F1_score">F1 score</a>, summarizing the number of correct positives and correct negatives out of all possible cases. In other words, how well does the model differentiate likely passes from failures?
- The size of the training set, preferring smaller training sets over larger ones. That is, how much data does the model need to make a reasonable prediction?
- The computation resources to make a reliable prediction. How much time and memory is required to correctly identify students that need intervention?

###Language and libraries
- Python 2.7
- Numpy
- Sklearn

###Dataset and template code
Download and unzip <a href="https://s3.amazonaws.com/content.udacity-data.com/courses/nd009/projects/student_intervention.zip">student_intervention.zip</a>. It should contain:

`student_intervention/`

- `README.md` - some notes about the dataset, including attribute meanings
- `student_intervention.ipynb` - iPython notebook with starter code
- `student-data.csv` - the student performance data

Open the iPython notebook, and follow along with instructions below.

###Deliverable
iPython notebook with all the steps marked with TODOs completed, and code blocks executed, showing desired outputs.
Project report in PDF format (3-5 pages), answering the following questions.

###1. Classification vs Regression

Your goal is to identify students who might need early intervention - which type of supervised machine learning problem is this, classification or regression? Why?

###2. Exploring the Data
Can you find out the following facts about the dataset?
Total number of students
Number of students who passed
Number of students who failed
Graduation rate of the class (%age)
Number of features
Use the code block provided in the template to compute these values.

###3. Preparing the Data
Execute the following steps to prepare the data for modeling, training and testing:
Identify feature and target columns
Preprocess feature columns
Split data into training and test sets
Starter code snippets for these steps have been provided in the template.

###4. Training and Evaluating Models
Choose 3 supervised learning models that are available in scikit-learn, and appropriate for this problem. For each model:
What is both the theoretical space complexity to represent the model and the time for the algorithm to make a prediction? You can either provide the big-O notation, or list several the of major features that may affect the algorithm and state if the largest driving factor is constant, linear, logrithmic, polynomical, etc in nature.
What are the general applications of this model? What are its strengths and weaknesses?
Given what you know about the data so far, why did you choose this model to apply?
Fit this model to the training data, try to predict labels (for both training and test sets), and measure the F1 score. Repeat this process with different training set sizes (100, 200, 300), keeping test set constant.
Produce a <a href="https://docs.google.com/document/d/1Goxw-6M0umOCokCFqTr-g7SU_5f6MIm_wqXmh9Cnjhw/pub" target="_blank">table</a> showing training time, prediction time, F1 score on training set and F1 score on test set, for each training set size.<br>
**Note**: You need to produce 3 such tables - one for each model.

###5. Choosing the Best Model
Based on the experiments you performed earlier, in 1-2 paragraphs explain to the board of supervisors what single model you chose as the best model. Which model is generally the most appropriate based on the available data, limited resources, cost, and performance?
In 1-2 paragraphs explain to the board of supervisors in layman’s terms how the final model chosen is supposed to work (for example if you chose a decision tree or support vector machine, how does it make a prediction).
Fine-tune the model. Use gridsearch with at least one important parameter tuned and with at least 3 settings. Use the entire training set for this.
What is the model’s final F1 score?

### Evaluation

Your project will be reviewed by a Udacity reviewer against **<a href="https://docs.google.com/document/d/1eyMT5SkhK4qiiFfTz1TrSnSqkV9gbH8g0Jfh3kW6apI/pub" target="_blank"> this rubric</a>**. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass.

### Submission
When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 2, and we'll walk you through the rest of the submission process.

If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **project@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.

### What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!
