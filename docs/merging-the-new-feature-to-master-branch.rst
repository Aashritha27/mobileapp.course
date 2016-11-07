Merging the New Feature to Master Branch
========================================

So now we are ready to push our change to master. I would type the following commands in my terminal, then creating a pull request in GitHub.

.. code::
  
  cd <my git folder>
  git add .
  git commit -am "Hyperlink Feature"
  git checkout master
  git pull
  git checkout feature/hyperlink
  git merge master
  git push origin feature/hyperlink

Creating and Merging Pull Request
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Pull request allows your teammates to review our change before it is merged into the master. Here are some links for background understanding on how does it work:

#. `About Pull Request <https://help.github.com/articles/about-pull-requests/>`_
#. `Creating a Pull Request <https://help.github.com/articles/creating-a-pull-request/>`_
#. `Merging Pull Request <https://help.github.com/articles/merging-a-pull-request/>`_
#. `Our Pull Request <https://github.com/pythonicbridge/mobileapp.kivy/pull/1>`_

Next
~~~~

Let's make a new release 0.2.0 as a next step.
