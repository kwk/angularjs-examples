Example 002 Authors with search
===============================

Based on the previous example we'll add a the ability to search for an author in the list. You type in a text and the unordered list of authors then shows only those authors matching your input. For the time being we don't care about the actual type of matching algorithm that is used. 

For this to work we introduce the concept of "filters" in AngularJS. Think of an expression where you print a value `{{ value }}` but before actually printing it you want to modify the value a bit.

AngularJS has some very powerful predefined filters like `currency` that basically displays numbers with two digits after the decimal point in a localized fashion.

To apply a filter in an expression you put at pipe symbol after the expression followed by the filter name. The filter might take additional options that are specified with a colon. Here's an example expression that prints a number in EURO: `{{ 23.4322 | currency:"EUR "}}` will print `EUR 23.43`.

In this example we want to search for a name in the list of authors. That's why it makes sense to use the `filter` filter from AngularJS. We create a new text input field and bind it's value to the `searchTerm` by using the `ng-model` directive. The authors are then filtered using only a slight modification to the author's listing: `{{ author in authors | filter:searchTerm }}`.

Notice that the filtering is happening immediately as you type! Cool, eh?
