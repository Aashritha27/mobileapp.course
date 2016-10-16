==========================================================
Current Solution: Strengths, Weaknesses, and Opportunities
==========================================================

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Strengths of Current Solution
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. Git and GitHub provides a platform for teachers to concurrently author the content, and have all changes versioned.
#. GitHub and ReadTheDocs works perfectly together to continously push the latest content available to the learners.
#. GitHub and ReadTheDocs are free, such that there is no cost of hosting and no server to be maintained.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Weaknesses of Current Solution
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. GitHub and ReadTheDocs can only host static content, which limits the interactivity of the course. As a programming class it is ideal to allow students editing and running programming quiz without leaving the course. Existing in-browser solutions are either `lack of 3rd party libraries support <http://www.skulpt.org/>`_, or `requires running and maintaining expensive servers <http://runestoneinteractive.org/>`_, which are not ideal to be plugged into the our current solution.
#. The current solution is web-based, and is inheriently less responsive than mobile app.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Opportunities to Improve Current Soution
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. Build a mobile learning app which synchronize static content from GitHub / ReadTheDocs, and run programming quizzes inside mobile device.
#. With Python and Kivy is possible to build a Python programming environment like  `this Android app <https://play.google.com/store/apps/details?id=enurisoft.com.pythoninterpreter&hl=en>`_. As the program is executed inside an Android phone, we can preload the 3rd libraries required, and the program can be run natively in an Android phone without a need of any expensive server.

With these opportunies, let's foucs on the requirements of our mobile learning app.
