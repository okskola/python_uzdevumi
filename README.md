# Python exercises with automated results testing
#### Video Demo:  https://youtu.be/v3dHIMK5isU
#### Author Ojārs Krūmiņš https://www.linkedin.com/in/ojars-krumins-0a367b6/
#### Motivation:
I teach programming (coding) at school so I wanted to create a web page where pupils could write some code and my page could automatically check for correct output.
There are multiple similar pages on the Internet, but usually they focus on some specific tasks or have more advanced tasks than my pupils can do. Also I wanted this page to be independent of some specific web server. What I wanted is to create a page where even simplest tasks, like creating a simple "Hello, world!" code could be checked.
#### Description:
This is a page where pupils can choose a task from a list, read the task, code it, run it and get automated result "pass" or "fail". The written code is automatically saved into browsers local storage when changing task or running it. The text on the page is written in Latvian.
How to use it:
-Start Python (Ieslēgt Python)
-Select a task (Izvēlies uzdevumu)
-Read the task (Uzdevuma teksts)
-Write the code
-Run the code (Izpildīt)
-Check the result (Rezultāts):
 -Pass (Pareizi)
 -Fail (Nepareizi)
-Delete all code from browsers local storage (Dzēst visu programmu kodus)
#### Files created and libraries used
-index.html: the main and only file (that was my intention to give pupils only one file) with html+css+js
-python_uzdevumi.json: JSON file with tasks (I was thinking to include these into HTML as well)
-favicon.ico: icon to display on web page
-ace,pyscript.*: saved versions of Ace editor and Pyscript just in case the authors change something which breaks my code
-The page uses Ace editor (https://ace.c9.io/) and PyScript (https://pyscript.net/) to let pupils write and execute Python code in a browser. I also added support of importing tasks through JSON file. Both Ace editor and PyScript has very little documentation so it took a lot of time to figure out how to use them for my specific needs.
#### This project can be further improved by:
- adding tasks editor for me or other teacher,
- adding ability to check for multiple inputs and outputs of the same task,
- improving visual design  (though I think that this is not important for such page),
- improve structure of the JavaScript code.
#### Problems
During writing of this code, the PyScript library changed so I had to adapt my code to use the new functionality. Before December 13, it was possible to redirect output of Pythons print() function to an HTML element, but now it always outputs to an element, created by PyScript itself. And I could not find the previous version of PyScipt library files. That is why I include current PyScript library code in my Github account, hoping that this will continue to work in future. This is also a reason why I did not made many tasks at the moment, because there is a risk that PyScript changes something again which will break my code and the time spend creating this will be useless. That is exactly what happened with ReplIt, when I had a classroom with exercises, but Replit changed the system and all my exercises are gone.