Example 003 Authors and books
=============================

Let's extend our model of authors. Currently we only store a simple array of strings in the `authors` array. We want to make this an array of objects with a list of books stored for each author.

Up until know we've stored everything inside our `index.html` file. Now is the time to introduce another file (`app.js`) in which we're going to put some of our JavaScript code. This should help unclutter out HTML file.

AngularJS supports the "Model View Controller" (MVC) patttern. which is sort of common sense nowadays to organize your data (model), the way it is modified (controller), and displayed on the screen (view). Currently our model only consists of this `authors` array and the view is the HTML. The controller is really only present in the form of the `filter:searchTerm` and the corresponding input field.

In the `app.js` file we will wrap our code inside a closure `(function(){  /* OUR CODE */ })();` which is also quite common and I'm not going into the details of it. Simply take it for granted and let's focus on the important part inside this closure.

Before we can go into the details of creating a simple AngularJS controller we've got to create a so called AngularJS [module][angular.moduule]:

> A module is a collection of services, directives, controllers, filters, and configuration information.

As a replacemend for the simple `authors` array, we will create an AngularJS [controller][understanding.controllers] and we're going to call it `AuthorsController`.

[angular.module] https://docs.angularjs.org/api/ng/function/angular.module "AngularJS Module"
[understanding.controllers] https://docs.angularjs.org/guide/controller "Understanding Controllers"
