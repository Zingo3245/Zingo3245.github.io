## Metis Live Online Introduction to Data Science Repo

Course materials for [Metis' Live Online Introduction to Data Science Course](http://www.thisismetis.com/introduction-to-data-science) (10/03/17 - 11/09/16).

**Instructor:** [Sergey Fogelson](https://www.linkedin.com/in/sergeyfogelson)

### [Course Project](project/README.md)

###Schedule:

Tuesday | Thursday
--- | ---
10/03: [Introduction to Python and Version Control](#class-1-introduction-to-python-and-version-control) | 10/05: [Introduction to Linear Algebra and Statistics in Python](#class-2-introduction-to-linear-algebra-and-statistics-in-python)

### Before the Course Begins (Prework):
* Install [Git](http://git-scm.com/downloads).
* Create an account on [GitHub](https://github.com/).
    * It is not necessary to download "GitHub for Windows" or "GitHub for Mac"
* Install [SourceTree](https://www.sourcetreeapp.com) and sign into your github account through it.
* Install [slack](https://slack.com) and get the necessary credentials to communicate on the metis slack channels.
* Install the [Anaconda distribution](http://continuum.io/downloads) of Python 2.7x.
    * If you choose not to use Anaconda, here is a list of the [Python packages](utils/python_packages.md) you will need to install prior to starting the course.
* Complete exercises 1-7, 13, 18-21, 27-35, 38, 39 of [Learn Python The Hard Way](http://learnpythonthehardway.org/book/)
* Watch the [linear algebra review videos](https://class.coursera.org/ml-005/lecture/preview) from Andrew Ng’s excellent Coursera ML course. They are labeled III. Linear Algebra Review (Week 1).
* Complete the exercises in chapters 2 and 3 of [this open textbook](https://www.openintro.org/stat/textbook.php).
)
* Practice Python using the resources below if you get through everything else.
* I would like to check the setup of your laptop before the course begins:
    * We need to figure out the logistics behind this, but it absolutely must happen before the course starts. If I cannot check it, someone else at Metis will, who will then sign off on you being able to start the course. YOU CANNOT START THE COURSE UNTIL EITHER I OR SOMEONE ELSE AT METIS CONFIRMS YOU HAVE A WORKING DEVELOPMENT ENVIRONMENT AS WE DO NOT WANT TO SPEND THE FIRST HOUR OF THE FIRST CLASS DEBUGGING ENVIRONMENTS.

### Python Resources
* [Codecademy's Python course](http://www.codecademy.com/en/tracks/python): Good beginner material, including tons of in-browser exercises.
* [DataQuest](https://dataquest.io/): Similar interface to Codecademy, but focused on teaching Python in the context of data science.
* [Google's Python Class](https://developers.google.com/edu/python/): Slightly more advanced, including hours of useful lecture videos and downloadable exercises (with solutions).
* [A Crash Course in Python for Scientists](http://nbviewer.ipython.org/gist/rpmuller/5920182): Read through the Overview section for a quick introduction to Python.
* [Python for Informatics](http://www.pythonlearn.com/book.php): A very beginner-oriented book, with associated [slides](https://drive.google.com/folderview?id=0B7X1ycQalUnyal9yeUx3VW81VDg&usp=sharing) and [videos](https://www.youtube.com/playlist?list=PLlRFEj9H3Oj4JXIwMwN1_ss1Tk8wZShEJ).
* [Python Tutor](http://pythontutor.com/): Allows you to visualize the execution of Python code.

### [Additional resources](#bonus-resources)

-----
### Class 1: Introduction to Python and Version Control
* Welcome
* Briefly discuss the [course project](project/README.md) and [public data sources](project/public_data.md)
* Intro to [SourceTree](https://www.sourcetreeapp.com)
* Intro to IPython Notebooks ([notebook](notebooks/01_intro_to_ipython_notebook.ipynb))
* Intro to Python ([notebook](notebooks/01_intro_to_python.ipynb))
* Wrap up: Getting help, course schedule, office hours

**Homework:**
* Finish whatever exercises from [LPTHW](http://learnpythonthehardway.org/book/) you couldn't finish. I assigned a lot of exercises as prework, so I suspect you have some things to work on. Focus on those concepts in the lecture that you didn't quite get.
* If your laptop has any setup issues, please work with me or someone else at Metis to resolve them by Thursday.

**Git Resources (IF YOU DON'T WANT TO USE SOURCETREE):**
* [Pro Git](http://git-scm.com/book/en/v2) is an excellent book for learning Git if you don't want to use SourceTree. Read the first two chapters if you want to gain a deeper understanding of version control.
* If you want to really practice a lot of Git (and learn many more commands), try [Git Immersion](http://gitimmersion.com/).
* [GitRef](http://gitref.org/) is an excellent reference guide for Git commands.

-----

### Class 2: Introduction to Linear Algebra and Statistics in Python
* Introduction to Linear Algebra in Python ([notebook](notebooks/02_intro_linalg.ipynb))
* Introduction to Statistics in Python ([notebook](notebooks/02_intro_stats.ipynb))

**Homework:**
* Work through as much of the [NumPy quickstart guide](https://docs.scipy.org/doc/numpy-dev/user/quickstart.html) as you can.
* Work through the remainder of the statistics exercises in the prework.

-----

## Bonus Resources

### Pandas/SQL/Databases
* This [slide deck](https://github.com/justmarkham/DAT5/blob/master/slides/20_sql.pdf) provides a brief introduction to databases and SQL.
* The repository for this [SQL Bootcamp](https://github.com/brandonmburroughs/sql_bootcamp) contains an extremely well-commented SQL script that is suitable for walking through on your own.
* This [ipython notebook](http://nbviewer.ipython.org/github/podopie/DAT18NYC/blob/master/classes/17-relational_databases.ipynb) provides a shorter introduction to databases and SQL that helpfully contrasts SQL queries with Pandas syntax.
* [SQLZOO](http://sqlzoo.net/wiki/SQL_Tutorial), [Mode Analytics](http://sqlschool.modeanalytics.com/), and [Code School](http://campus.codeschool.com/courses/try-sql/contents) all have online beginner SQL tutorials that look promising.
* [w3schools](http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all) has a sample database that allows you to practice SQL from your browser. Similarly, Kaggle allows you to query a large SQLite database of [Reddit Comments](https://www.kaggle.com/c/reddit-comments-may-2015/data) using their online "Scripts" application.
* [What Every Data Scientist Needs to Know about SQL](http://joshualande.com/data-science-sql/) is a brief series of posts about SQL basics, and [Introduction to SQL for Data Scientists](http://bensresearch.com/downloads/SQL.pdf) is a paper with similar goals.
* [10 Easy Steps to a Complete Understanding of SQL](http://tech.pro/tutorial/1555/10-easy-steps-to-a-complete-understanding-of-sql) is a good article for those who have some SQL experience and want to understand it at a deeper level.
* SQLite's article on [Query Planning](http://www.sqlite.org/queryplanner.html) explains how SQL queries "work".
* [A Comparison Of Relational Database Management Systems](https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems) gives the pros and cons of SQLite, MySQL, and PostgreSQL.
* If you want to go deeper into databases and SQL, Stanford has a well-respected series of [14 mini-courses](https://lagunita.stanford.edu/courses/DB/2014/SelfPaced/about).
* [Blaze](http://blaze.readthedocs.org/en/latest/index.html) is a Python package enabling you to use Pandas-like syntax to query data living in a variety of data storage systems.

### Tidy Data is Better Data
* [Good Data Management Practices for Data Analysis](https://www.prometheusresearch.com/good-data-management-practices-for-data-analysis-tidy-data-part-2/) briefly summarizes the principles of "tidy data".
* [Hadley Wickham's paper](http://www.jstatsoft.org/v59/i10/paper) explains tidy data in detail and includes lots of good examples.
* Example of a tidy dataset:
    * [Bob Ross](https://github.com/fivethirtyeight/data/blob/master/bob-ross/elements-by-episode.csv)
* Examples of godawful/untidy datasets: 
    * [NFL ticket prices](https://github.com/fivethirtyeight/data/blob/master/nfl-ticket-prices/2014-average-ticket-price.csv)
    * [airline safety](https://github.com/fivethirtyeight/data/blob/master/airline-safety/airline-safety.csv)
    * [Jets ticket prices](https://github.com/fivethirtyeight/data/blob/master/nfl-ticket-prices/jets-buyer.csv)
    * [Chipotle orders](https://github.com/TheUpshot/chipotle/blob/master/orders.tsv)

In general, [spreadsheets that are unreadable by computers](https://bosker.wordpress.com/2014/12/05/the-government-statistical-services-terrible-spreadsheet-advice/) are the worst. 

If you (or your friends/colleagues) tend to make them, please [read this](http://www.clean-sheet.org/). There are additional suggestions for how to make tidy data [here](http://stats.stackexchange.com/questions/83614/best-practices-for-creating-tidy-data/83711#83711).
