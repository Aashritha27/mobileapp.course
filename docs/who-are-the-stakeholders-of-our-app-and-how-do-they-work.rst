========================================================
Who Are the Stakeholders of Our App and How Do They Work
========================================================

Let's begin by taking a look on how the following stakeholders use this course web site, as a course authoring and publishing workflow:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
How Educations and Learners Are Connected Together
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. Educators may update course material via `GitHub <https://github.com/pythonicbridge/mobileapp.course/tree/master/docs>`_.
#. Once the educators has `committed the changes to GitHub <https://help.github.com/articles/editing-files-in-your-repository/>`_, GitHub will `trigger a webhook to ReadTheDocs <http://docs.readthedocs.io/en/latest/webhooks.html>`_.
#. ReadTheDocs would parsee the course material written in `reStructuredText language <http://www.sphinx-doc.org/en/stable/rest.html>`_, and convert them into HTML with navigation menu, themes, and cosmestics.
#. Learners may visit `the course home page <http://pythonic-cs1-build-a-mobile-app.readthedocs.io/>`_ to access the latest course content.

Next, we can compare and contrast the strengths and weaknesses of this solution.
