Requirements of Our Mobile Learning App
=======================================

Let's drill down in detail for the requirements:

#.	We are currently hosting our course homepage in GitHub. GitHub is a version control system that allows collaborators to contribute content and code concurrently in a common repository. GitHub allows static content like articles and videos to be hosted and navigated via ReadTheDocs web interface. A requirement of the Mobile Learning App is to download the latest content from GitHub and display it as clickable menu item accordingly. Each menu item has an ID and description.
#. Each page of course content is presented sequently to learners. For article content, it is scrollable vertically. User can click on previous / next button for its corresponding previous / next screen of content. We do not have much Video content currently so let's assume we are hosting only text content for now.
#. For programming quiz, a text editor is presented with the starter code and the learner would complete the program. There is a "Run Test" button which check the correctness of the program by executing it locally in the Android phone.
#. For the last page of the screen, the next button will bring the menu screen. Similarly, for the first page of the screen, the previous button will bring the menu screen.
