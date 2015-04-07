Students will develop a database schema to store the game matches between players. Students will then write a Python module to rank the players and pair them up in matches in a tournament.

## How will students complete this project?

1. Install [Vagrant](http://vagrantup.com) and [VirtualBox](https://www.virtualbox.org/)
2. Clone the [fullstack-nanodegree-vm repository](http://github.com/udacity/fullstack-nanodegree-vm)
3. Launch the Vagrant VM
4. Write SQL database and table definitions in a file (`tournament.sql`)
5. Write Python functions filling out a template of an API (`tournament.py`)
6. Run a test suite to verify your code (`tournament_test.py`)

For complete project details, make sure you check out <a href="https://www.udacity.com/course/viewer#!/c-ud197/l-3521918727/m-3554068605" target="_blank">Lesson 5</a> of the Intro to Relational Databases course, including the <a href="https://www.udacity.com/course/viewer#!/c-ud197/l-3521918727/m-3519689284" target="_blank">Project Description</a>.

## Things to watch out for

The rubric specifies that the code "makes use of query parameters appropriately to protect against SQL injection attacks."
This means that students should use the `execute` method, not string concatenation or interpolation to assemble their queries.
Refer to the the [psychopg docs](http://initd.org/psycopg/docs/usage.html#the-problem-with-the-query-parameters) for why.

This does __NOT__ mean that students should use the Bleach library to sanitize inputs.
Since this project doesn't involve HTML and the database doesn't store HTML there is no good reason to use Bleach.
