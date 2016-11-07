Making Another Release
======================

Let's make a new release. This can be done by the following.

.. code::
  
  cd <my git folder>
  git checkut master
  git pull
  git checkout -b release/0.2.0
  git push origin release/0.2.0
  
Making a release has the following advantages:

#. At the end of each module for this course, we have create a new release branch. This way, students can refer to where they are as a snapshot to compare what has been changed from 1 module to the other.
#. Similarly, for our Mobile Learning App as a software product, we also make release for each set of feature(s) we have added, such that we can fallback to previous version if there is any issue.
