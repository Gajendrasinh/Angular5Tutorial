# Angular5Tutorial
angular 5 tutorial for beginners

# How to Install Angular 5

Prerequisites

You're going to need a couple things before proceeding:

    Node.js
    Node Packange Manager (NPM)

To check whether or not you have both of these installed, visiting your command line or console and type:

    $ node -v
    $ npm -v
    
Installing Angular 5 through the CLI

The Angular CLI (Command Line Interface) is the quickest and easiest way to get started with a brand new Angular 5 project. 

We're going to use NPM (you can also use yarn) to install the Angular CLI through the following command:

    $ npm install @angular/cli -g

Once installed, you can access the CLI tool by typing ng.

To check the version of your Angular CLI, type:

    $ ng -v
    
now we're ready to use the CLI to start the project.
 
    $ ng new my-ng5-project  --routing
 
The one flags we added at the end specify that we want the --routing tells the CLI to provide us with the routing scaffolding.

It will run for awhile and then prompt you that you can cd into the new project folder. To do that, simply type

    
    $ cd my-new-project
    
To serve your project in the browser, which is useful for development as it automatically compiles your project and reloads it in the browser, type:

    $ ng serve
    
Now You have a fresh copy of Angular 5 ready and waiting for you to develop.
