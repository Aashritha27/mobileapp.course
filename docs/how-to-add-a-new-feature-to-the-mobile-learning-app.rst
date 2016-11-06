How to Add a new Feature to the Mobile Learning App
===================================================

In this module, we would like to demostrate on how to add a new feature to the mobile learning app. Imagine the following scenario and goals:

#. You and me are assigned to develop new features for the mobile learning app.
#. I am developing a new feature to support external hyperlink. I will show you how I do it.
#. You are developing a new feature to support images. You are developing it while I am also developing my feature concurently.
#. Once your changes and my changes are ready, we will create a new release, namely 0.2.0.
#. If you remember, we are having our last release as 0.1.0. So here we would like to make sure our changes will only be visible right after 0.1.0 and will be releasd in 0.2.0.

Here we would like to outline what we should do to achieve the goals above:

#. Create a git feature branch from git master.
#. Create 1 more test cases for the new feature we are adding. Build our feature to pass the test case.
#. Integrating changes into master
#. Create a release branch from master when my change and your chnages are ready.

Let's walk though them step-by-step.
