How to Implement a Programming Quiz in Our Mobile Learning App
==============================================================

Road Map
~~~~~~~~

Recall the steps we need to implement a new feature to our app:

#. Understand our requirements.
#. Implement the user interface.
#. Write a test case.
#. Implement the test case to pass the test.
#. Integrate our change.

We will follow the steps exactly to implement the programming quiz feature. Due to the time constraints, for now we will disucss the high level design and leave the actual implementation as an exercise for the students.

Requirements
~~~~~~~~~~~~

As usual we will read the RST file for their instruction. For simplicity, assume we have the following RST content:

.. code:: rst

  .. code:: python
  
    # PROGRAMMING QUIZ
    
    import unittest
    
    def say(something):
      return something
    
    class ProgrammingQuiz(unittest.TestCase):
      def test1():
        self.assertEqual('Hello world', say_hello('Hello world'))

When we intrepret the code directive, followed by # PROGRAMMING QUIZ comment, our application should be:

#. Replace the whole code block as a ref, similar to what we did for hyperlink.
#. We should also store everything found in this block into a `CodeInput <https://kivy.org/docs/api-kivy.uix.codeinput.html>`_ box such that it allows student to start editing the source code to complete the programming quiz.
#. We should also provide buttons for students to (1) start over, (2) execute the code by running the unittest.main() and present the result, (3) go back to the page which triggers the programming test.
