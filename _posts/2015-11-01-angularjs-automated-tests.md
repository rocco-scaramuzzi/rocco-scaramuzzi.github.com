---
layout: post
category: lessons
tagline: Supporting tagline
tags: 
  - intro
  - beginner
  - jekyll
  - tutorial
published: true
---




{% include JB/setup %}

Several scientific studies demonstrated that automated tests allow to reduce a lot the costs to develop and maintain an application as well as they allow to improve the quality of the software.

Nowadays the web applications become more and more complex at the client side than before. That allowed javascript framework as AngularJS to became very popular and essentials to build well designed web applications with 100% of separation of concerns. 

If we have a web application with a complexity at the client side it easy to understand how important the automated tests can be to develop and maintain our application.

One of the most common tools which allows to build automated unit test in JavaScript is [Karma](http://karma-runner.github.io/0.13/index.html). Although Karma has been created by the AngularJS team, it is a test runner which can be used to test any JavaScript application. Of Course it is too much easier to use Karma for JavaScript applications written using AngularJS since AngularJS has been designed keeping in mind the possibility to make the client side testable as the server side.

Karma runs on nodeJS, below there is a summury schema about how Karma works, for more details plese check the karma web site on this [section](http://karma-runner.github.io/0.13/intro/how-it-works.html).

![]({{site.baseurl}}/_posts/images/karma-how-works.jpg?raw=true)

Karma test runner generates a web server that executes source code against test code for each of the browsers connected to it. Karma support allow to run unit test written in different frameworks, the one I am using is Jasmine. The results for each test against each browser are examined and displayed via the command line to the developer such that they can see which browsers and tests passed or failed. All the information as the kind of unit tests, the browser/browsers used to run the tests etc are defined during the installation of Karma inside the local project.




Conclusion

- Karma as unit tests
- Karma schema
- Karma installation
- Conclusion: Unit test allow us to write better test
