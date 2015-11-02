---
layout: post
category: client side
tags: 
  - angularjs
  - unit test
  - karma
published: true
---




{% include JB/setup %}

Several scientific studies demonstrated that automated tests allow to reduce a lot the costs to develop and maintain an application as well as they allow to improve the quality of the software.

Nowadays the web applications become more and more complex at the client side than before. That allowed javascript framework as AngularJS to became very popular and essentials to build well designed web applications with 100% of separation of concerns. 

If we have a web application with a complexity at the client side it easy to understand how important the automated tests can be to develop and maintain our application.

One of the most common tools which allows to build automated unit test in JavaScript is [Karma](http://karma-runner.github.io/0.13/index.html). Although Karma has been created by the AngularJS team, it is a test runner which can be used to test any JavaScript application. Of Course it is too much easier to use Karma for JavaScript applications written using AngularJS since AngularJS has been designed keeping in mind the possibility to make the client side testable as the server side.

Karma runs on NodeJS, below there is a summury schema about how Karma works, for more details plese check the karma web site on this [section](http://karma-runner.github.io/0.13/intro/how-it-works.html).

![How it works](https://raw.githubusercontent.com/rocco-scaramuzzi/rocco-scaramuzzi.github.com/master/_posts/images/karma-how-works.jpg)

Karma test runner generates a web server that executes source code against test code for each of the browsers connected to it. Karma support allow to run unit test written in different frameworks, the one I am using is [Jasmine](http://jasmine.github.io/2.0/introduction.html). The results for each test against each browser are examined and displayed via the command line to the developer such that they can see which browsers and tests passed or failed. All the information as the kind of unit tests, the browser/browsers used to run the tests etc are defined during the installation of Karma inside the local project.

In order to install karma you do need to have NodeJS installed on your machine. Once you got NodeJS, run locally to your project folder the following commands:
 
### Install Karma:
$ npm install karma --save-dev
  
### Install plugins that your project needs:
$ npm install karma-jasmine karma-chrome-launcher --save-dev

### Install karma command line globaly
$ npm install -g karma-cli
 
Those commands will install _karma_, _karma-jasmine_ and _karma-chrome-launcher_ packages into node_modules in your project directory and also save these as devDependencies in package.json, so that any other developer working on the project will only have to do npm install in order to get all these dependencies installed. The last command allow to install karma globally so that we can run it from anywhere.

Configuring Karma consist in creating the default karma.conf.js file on the root of our project folder. For more details please have a look the ufficial [Karma configuration](http://karma-runner.github.io/0.12/intro/configuration.html) page. 

In the next article I will show how easily we can write unit tests (using Jasmine) and use Karma to run them.

Bye!!!
