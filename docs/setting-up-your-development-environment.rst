Setting up Your Development Environment
=======================================

Let's get the hands dirty by doing some setup. We will explain what you have done later. Just feel free to try it out for now :)

Download and Install
~~~~~~~~~~~~~~~~~~~~

#. Download and install `Virtual Box <https://www.virtualbox.org/>`_.
#. Download and add `Ubuntu 64 Bit Virtual Box image <http://www.osboxes.org/ubuntu/>`_ into your Virtual Box. Latest version is recommended. Please refer to the web site for user name and password.

Commands to be Run
~~~~~~~~~~~~~~~~~~

#. Start the Ubuntu. Input the username and password obtained in the last step to login. Right click desktop and choose open terminal.
#. In the terminal, run the following command:

.. code::

  sudo apt upgrade
  sudo apt install python-kivy
  sudo apt install git
  sudo apt intall pip

Intall Pycharm IDE
~~~~~~~~~~~~~~~~~~

#. In your Ubuntu. Open Firefox. And download `PyCharm Commnity Edition for Linux<https://www.jetbrains.com/pycharm/download/#section=linux>`_
#. By default, it would be saved at ~/Downloads.
#. Open terminal again. Type the following:

.. code::

  cd ~/Downloads
  tar xvzf pycharm*.tar.gz
  rm pycharm*.tar.gz
  mv pycharm* ~/pycharm

Running PyCharm
~~~~~~~~~~~~~~~

#. Open terminal.
#. Run Pycharm in terminal by:

.. code::

  ~/pycharm/bin/pycharm.sh

In the next section. You will learn about what you have just setup.
