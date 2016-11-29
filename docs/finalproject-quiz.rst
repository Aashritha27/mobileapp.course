Final Project: Sample Programming Quiz
======================================

Sample Programming Quiz
~~~~~~~~~~~~~~~~~~~~~~~

If you implement the things correctly, the following code block will become a link the a programming quiz when your mobile app visit this page:

.. code:: python

  # PROGRAMMING QUIZ
  
  import unittest2
  
  def say_hello(something):
    return something
  
  class ProgrammingQuiz(unittest2.TestCase):
    def test_say_hello(self):
      self.assertEqual('Hello world', say_hello('world'))
  
  # END OF PROGRAMMING QUIZ

And the screen would look something like this:

.. image:: programming-quiz.png

Reference Implementation
~~~~~~~~~~~~~~~~~~~~~~~~

Due to the time constraint, we do not provide a reference implementation for this one (as planned). We might consider implementing one if time is still allowed. Stay tuned :)
