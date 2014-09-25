***DESCRIPTION***

The views folder contains the LEAPTEST.HTML FILE that consists of the entire sample,
which could be run locally simply by opening the html file in a web browser.
However, for the project structure to be deployed to the web via Heroku,
there are other files necessary as well. The other file in the views folder is the
LEAPTEST.JADE FILE, which is simply a pointer file to the html file (will be explained
in a minute).

The APP.JSON FILE just has a brief description of the application as well as where it
can be found online and a few other details.

The INDEX.JS FILE is reading the .jade file, which tells it to instead render the.html
file. This file uses Express -- a Sinatra-like minimal and flexible node.js web
application framework -- and will be added to in much greater detail as the application
progresses.

The PACKAGE.JSON FILE gives a description of the application, declares the main
javascript file to start at, as well as states node.js dependencies and the engine
(and versions of all these things).



***HELPFUL HINTS***
When using new modules of node.js, it will be required to add the appropriate dependency
to the PACKAGE.JSON file. You are using a new module whenever in the .js file (typically 
at the top of the file), you have: var __varName = require('__someDependency'). This means
that __someDependency is a module that needs to be added to the dependency list in the
PACKAGE.JSON file, following the same format as for the other modules. To find out the
most up-to-date version, in the terminal type:   npm show {__moduleName} version
where __moduleName is the same as __someDependency.
