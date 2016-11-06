How to Add a Unit Test
======================

What is and Why Unit Test
~~~~~~~~~~~~~~~~~~~~~~~~~

Unit test and `unit testing <https://en.wikipedia.org/wiki/Unit_testing>`_ are important concepts and activities that help us to write high quality code with productivity. Let's highlight the folowing advantages:

#. It allows part of our program to be test independently from ther others, hence helping us to focus on what we are testing.
#. Unit testing can be automated, hence giving us a ability of testing our program automatically.
#. It allows us to accumulate a suite of test cases. Imagine if I develop my feature with its corresponding test cases and you also do the same. Collectively we can test the different features of the program automatically.

Understanding Requirements
~~~~~~~~~~~~~~~~~~~~~~~~~~

Let's demostrate how to add a Unit to test the feature I am building, i.e. support of external hyperlink. Let's understand the requirements:

.. image:: raw-hyperlink.png

As you can see above, hyperlinks are not displayed properly in the screen. We would like to add support for hyperlink such that:

#. We would read the page line-by-line, and replace all \`link description \<link\>\`_ patterns such that they are instead become [ref=link]link description[/ref]. For example, the above link should be presented as [ref=https://en.wikipedia.org/wiki/Unit_testing]unit testing[/ref].
#. There can be 1 or more hyperlink within single line. Each of them should be handled accordingly.
#. Once clicked, a web browser should be launched to display the corresponding web page.

Let's add a Unit Test for parsing and formatting the hyperlink as required above. We will leave launching a web browser to be done in the next module.

Adding Unit Test with Pycharm
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. Add a method format_hyperlink(self, line) inside CourseApp class. For now, let's simply add return line as its implementation.
#. Add a file test_CourseApp.py. It should look like this.
