# Software Engineering

![c](https://user-images.githubusercontent.com/116082827/235298861-62ff4768-b591-4214-a9ad-20926c64037d.jpeg)


Software engineering is the process of designing, developing, testing, and maintaining software. It involves a range of best practices and methodologies, such as agile development, version control, and automated testing. Here's an example of a simple software engineering project in Python that uses the Pytest library for unit testing:



# main.py

def add(a, b):

    return a + b



# test_main.py

import pytest

from main import add



def test_add():

    assert add(2, 3) == 5

    assert add(0, 0) == 0

    assert add(-1, 1) == 0
