# Programming Foundations with Python

In the Project: _Movie Trailer Website_ part of the online syllabus, complete the following lessons in the Programming Fundamentals and the Web module:

* Introduction
* Use Functions
* Use Classes: Draw Turtles
* Use Classes: Profanity Editor
* Make Classes: Movie Website

Things I will probably be adding:

* Discussion of Github.  Probably will do a workshop so everyone is familiar with collaborating.  Run through codeschool's [Git training](https://www.codeschool.com/courses/try-git).
* Discussion of c9.io.
* Downloading of PyCharm Community Edition \(free and awesome\)
* Discussion of Python 2 vs Python 3.
* Installation of pyenv and a discussion of how to use it.
* Discussion of unit tests \(just the intro\)
* Downloading[ Python 3.6](https://www.python.org/)

### Steps:

* Download Python.

* Create a directory.

* Change to that directory.
  * run `python -m venv pyrepo`
  * run `source pyrepo/bin/activate`
  * run `pip install flake8 pytest hypothesis mypy`
  * run `pip freeze > requirements.txt`
* What this does is creates a virtual environment, \(we'll discuss in class\), then activates it, then pip install adds in four modules:  
  * Code Quality:  flake8 and mypy are for code linting.  
    * Flake8 is uses pep8, \(which is renamed now to `pycodestyle` to avoid confusion\), and pyflakes.   When you hear the instructors in video to run pep8, you should run `flake8` instead.
    * Mypy checks for code type-hinting.  If an invalid argument is used based on the code type-hint, mypy will warn you about it.
  *  pytest and hypothesis are for testing code.
    * pytest is a very simple testing framework that is much easier to use than the default that comes with Python.
    * Hypothesis is what's known as a `mutator check`.  This means it puts multiple mutations in the code to see if the code reacts the way it is expected, according to the test.



