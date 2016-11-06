How to Create a Feature Branch in Git
=====================================

Steps
~~~~~

Let's demostrate the first step by creating a new feature branch from master. First I will type the following from my terminal

.. code::

  cd <<your git clone folder>>
  git checkout master
  git pull
  git checkout -b feature/hyperlink
  
The command above will:

#. Get the latest code from master
#. Create a new feature branch from master, namely feature/hyperlink.

I can verify I am in my feature branch by typing:

.. code::

  git branch
  
It will highlight my current branch.

Why a Feature Branch
~~~~~~~~~~~~~~~~~~~~

The followings are reasons why we make a feature branch from master:

#. It allows me to develop my feature without impacting the others.
#. It allows me to select a right moment, where my changes are ready and tested, to be integrated into master with other people changes to collectively make a new release.

Discussions
~~~~~~~~~~~

#. Note the arrangement above is just one possible way of branching. As our project is simple we choose simple model.
#. You may `watch this video <https://www.atlassian.com/agile/branching>`_ for some other advanced branching models.
