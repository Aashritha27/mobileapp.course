Optional: How to build an App Which is Ready for Deployment into Google Play Store
==================================================================================

So far we have been using Kivy Launcher to run our main.py file without any compliation. It works great for development. But if we want to deploy the app as a standalone program into Google Play Store, we need a way to build an `APK Package <https://en.wikipedia.org/wiki/Android_application_package>`_. APK Package is a package that contains the following information:

#. The compiled binary files and libraries required for the app.
#. A manifest file describing the attributes for the app, such as orientation, permission needed, etc.

Kivy has a mechanism called buildozer that help us creating this package. Let's see how does it work.

Step 1: Install Buildozer
~~~~~~~~~~~~~~~~~~~~~~~~~

.. code::

  sudo pip install buildozer
  sudo dpkg --add-architecture i386
  sudo apt-get update
  sudo apt-get install build-essential ccache git libncurses5:i386 libstdc++6:i386 libgtk2.0-0:i386 libpangox-1.0-0:i386 libpangoxft-1.0-0:i386 libidn11:i386 python2.7 python2.7-dev openjdk-8-jdk unzip zlib1g-dev zlib1g:i386

Step 2: Setup Buildozer for Our Mobile App
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code::

  cd <your app folder>
  buildozer init
  vi buildozer.spec

This will open the buildozer.spec file. You may change permission / libraries needed in here. `Click here for details <http://buildozer.readthedocs.io/en/latest/specifications.html>`_.

Step 3: Run Buildozer
~~~~~~~~~~~~~~~~~~~~~

.. code::

  buildozer -v android debug

This will start the compilation. The first run will take long as it will download `Android SDK <https://developer.android.com/studio/index.html>`_ and `Android NDK <https://developer.android.com/ndk/index.html>`_. The subsquent run will be much faster.

Once the complication is done you should be able to see an apk file in <your app dir>/bin folder. You may use upload this file into your Google Drive and download it into your phone. Click on the APK file to install. If you ask for permission, grant it and it should complete the installation.

Step 4: Upload to Google Play Store (optional)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Click here <https://support.google.com/googleplay/android-developer/answer/113469?hl=en>`_ for details. This step is optional as you need to pay google momey to do it :)

Additional Resources
~~~~~~~~~~~~~~~~~~~~

#. `Kivy Crash Course: Buildozer <https://www.youtube.com/watch?v=t8N_8WkALdE>`_
#. `Android Permissions <https://developer.android.com/guide/topics/security/permissions.html>`_
