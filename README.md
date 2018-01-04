# Angular 5 Tutorial
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

    
    $ cd my-ng5-project
    
To serve your project in the browser, which is useful for development as it automatically compiles your project and reloads it in the browser, type:

    $ ng serve
    
Now You have a fresh copy of Angular 5 ready and waiting for you to develop.


What are Components?

Angular components are the basic building blocks of your app. Each component defines:

Any necessary imports needed by the component
A component decorator, which includes properties that allow you to define the template, CSS styling, animations, etc..
A class, which is where your component logic is stored.

Angular components reside within the /src/app folder:

    > src
      > app
        app.component.ts  
        app.component.html   
        app.component.scss  

By default, the Angular CLI that we used to install the project just includes the /src/app/app.component files. A little later on, we will use the CLI to generate a new component for us and you will see how the folder structure reacts.

# The Basic Component File

    import { Component } from '@angular/core';

    @Component({
      selector: 'app-root',
      templateUrl: './app.component.html',
      styleUrls: ['./app.component.scss']
    })
    export class AppComponent {
      title = 'app';
    }

# Creating a New Component

    $ ng generate component contact or ng g c contact
    
    // Output:

    create src/app/contact/contact.component.html (23 bytes)
    create src/app/contact/contact.component.spec.ts (614 bytes)
    create src/app/contact/contact.component.ts (262 bytes)
    create src/app/contact/contact.component.scss (0 bytes)
    update src/app/app.module.ts (467 bytes)
