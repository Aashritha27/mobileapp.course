Final Project: Implement a Programming Quiz in Our Mobile Learning App
======================================================================

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
    
    def say_hello(something):
      return something
    
    class ProgrammingQuiz(unittest.TestCase):
      def test1():
        self.assertEqual('Hello world', say_hello('Hello world'))

When we intrepret the code directive, followed by # PROGRAMMING QUIZ comment, our application should be:

#. Replace the whole code block as a ref, similar to what we did for hyperlink.
#. We should also store everything found in this block into a `CodeInput <https://kivy.org/docs/api-kivy.uix.codeinput.html>`_ box such that it allows student to start editing the source code to complete the programming quiz.
#. We should also provide buttons for students to (1) start over, (2) execute the code by running the unittest.main() and present the result, (3) go back to the page which triggers the programming test.
#. We expect to have a seperate screen for programming quiz. You may check out `this video <https://www.youtube.com/watch?v=xx-NLOg6x8o>`_ on how to add another screen via Screen Manager in Kivy framework.
#. We should have a way to (1) execute the program, (2) output of test cases, either passing or failing. For (1), we can look at `this function <https://docs.python.org/2/library/functions.html#eval>`_. For (2) we can look at `this article <http://stackoverflow.com/questions/1218933/can-i-redirect-the-stdout-in-python-into-some-sort-of-string-buffer>`_ and `this documentation <https://docs.python.org/2/library/stringio.html>`_.

Technical Requirements
~~~~~~~~~~~~~~~~~~~~~~

#. After you have implemented your change, if you copy your main.py into your mobile phone, you will found that the mobile app cannot be run. It is due to that CodeInput box requires `Pygments <http://pygments.org/>`_ for its syntax highlighting function, but Pygments is missing in Kivy launcher. To handle this, you may either (1), Fallback to Text Input (by adding a `import fallback handler <http://stackoverflow.com/questions/3131217/error-handling-when-importing-modules>`_), (2) or add Pygments dependency and build via Buildozer as mentioned in the next page.
#. (Optional) Ideally, we should provide a way to store and retrieve the programing quiz history such that students can track and revise later. Ideally, we should be able to leverage `GitHub Gist <https://gist.github.com/>`_ for storage. This way, student and write their code on-the-go in cell phone, and carry on coding in front of desktop computer by checking out the Gist. Support of this feature is not hard but it involves a bit of integration effort. Cosider this as the final challenges :)

Starter Code / Test Cases
~~~~~~~~~~~~~~~~~~~~~~~~~

There is no starter code / start test cases for this time. You may refer to previous module on how to start :)

Sample Programming Quiz
~~~~~~~~~~~~~~~~~~~~~~~

If you implement the things correctly, the following code block will become a link the a programming quiz when your mobile app visit this page:

.. code:: python

  # PROGRAMMING QUIZ
  
  import unittest
  
  def say_hello(something):
    return something
  
  class ProgrammingQuiz(unittest.TestCase):
    def test1():
      self.assertEqual('Hello world', say_hello('Hello world'))

Reference Implementation
~~~~~~~~~~~~~~~~~~~~~~~~

Due to the time constraint, we do not provide a reference implementation for this one (as planned). We might consider implementing one if time is still allowed. Stay tuned :)
