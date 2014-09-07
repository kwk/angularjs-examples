Example 001 Authors
===================

In this introductory example, we'll be using the most basic but powerful features of AngularJS I can think of: directives and expressions.

In the `<html>` tag we'll tell AngularJS that this is going to be an AngularJS application by specifying the `ng-app` directive.

The whole point of this example is to have a good starting point upon which we can build at least some more examples later.

We'll start of with a simple list of author names and later add a whole lot to it that makes the website more interesting. 

In this first example we create an array of author names by specifying it with the `ng-init` directive. Then we use the `ng-repeat` much like a for-loop to iterate over the list of names. For every author this will add an `<li>` element to the unordered list.

To print each name we use what's called an "expression". Expressions are enclosed in two openening and two closing curly braces.

Notice, that in this example, we didn't write much JavaScript code at all. Only the array of authors is a JavaScript expression. The rest is all AngularJS magic.
