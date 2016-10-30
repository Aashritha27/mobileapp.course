Building the Mobile Learning App in Python and Kivy
===================================================

Let's back to to our focus on building a mobile learning app. Recapping what we have prototyped, we are building a mobile learning app which allows contributor to create / modify content via Git / GitHub. And the content can be sycnrhonized automatically to ReadTheDocs as well as our mobile learning app. Let's learn it by doing it.

Step 1: Fork the Starter Code into Your GitHub Account
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. Please fork from `this URL <https://github.com/pythonicbridge/mobileapp.kivy>`_. Please refer to the previous sections if you are not sure how to do it.

Step 2: Clone to PyCharm
~~~~~~~~~~~~~~~~~~~~~~~~

#. Like what we did previously. Please refer to the previous document for details.

Step 3: Run the Starter Code
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. By locating main.py and run it. You should see a screen like this:

.. image:: pythonic-cs1-kivy.png

The mobile learning app fetch the course content from GitHub and present it to the user. Navigation menu including Home, Up, and Next are working the similar way like our Prototype. Unlike the prototype, as `Kivy label supports ref and other markups <https://kivy.org/docs/api-kivy.core.text.markup.html>`_, we can embed the menu directly into the document such that it looks more natural.
