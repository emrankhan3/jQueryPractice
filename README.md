## Learn How Script Tags and Document Ready Work
Now we're ready to learn jQuery, the most popular JavaScript tool of all time.

Before we can start using jQuery, we need to add some things to our HTML.

First, add a script element at the top of your page. Be sure to close it on the following line.

Your browser will run any JavaScript inside a script element, including jQuery.

Inside your script element, add this code: $(document).ready(function() { to your script. Then close it on the following line (still inside your script element) with: });

We'll learn more about functions later. The important thing to know is that code you put inside this function will run as soon as your browser has loaded your page.

This is important because without your document ready function, your code may run before your HTML is rendered, which would cause bugs.

## Target HTML Elements with Selectors Using jQuery
Now we have a document ready function.

Now let's write our first jQuery statement. All jQuery functions start with a $, usually referred to as a dollar sign operator, or as bling.

jQuery often selects an HTML element with a selector, then does something to that element.

For example, let's make all of your button elements bounce. Just add this code inside your document ready function:

$("button").addClass("animated bounce");

Note that we've already included both the jQuery library and the Animate.css library in the background so that you can use them in the editor. So you are using jQuery to apply the Animate.css bounce class to your button elements.

## Target Elements by Class Using jQuery
You see how we made all of your button elements bounce? We selected them with $("button"), then we added some CSS classes to them with .addClass("animated bounce");.

You just used jQuery's .addClass() function, which allows you to add classes to elements.

First, let's target your div elements with the class well by using the $(".well") selector.

Note that, just like with CSS declarations, you type a . before the class's name.

Then use jQuery's .addClass() function to add the classes animated and shake.

For example, you could make all the elements with the class text-primary shake by adding the following to your document ready function:

$(".text-primary").addClass("animated shake");

## Target Elements by id Using jQuery
You can also target elements by their id attributes.

First target your button element with the id target3 by using the $("#target3") selector.

Note that, just like with CSS declarations, you type a # before the id's name.

Then use jQuery's .addClass() function to add the classes animated and fadeOut.

Here's how you'd make the button element with the id target6 fade out:

$("#target6").addClass("animated fadeOut");

## Delete Your jQuery Functions
These animations were cool at first, but now they're getting kind of distracting.

Delete all three of these jQuery functions from your document ready function, but leave your document ready function itself intact.

## Target the Same Element with Multiple jQuery Selectors
Now you know three ways of targeting elements: by type: $("button"), by class: $(".btn"), and by id $("#target1").

Although it is possible to add multiple classes in a single .addClass() call, let's add them to the same element in three separate ways.

Using .addClass(), add only one class at a time to the same element, three different ways:

Add the animated class to all elements with type button.

Add the shake class to all the buttons with class .btn.

Add the btn-primary class to the button with id #target1.

Note: You should only be targeting one element and adding only one class at a time. Altogether, your three individual selectors will end up adding the three classes shake, animated, and btn-primary to #target1.

## Remove Classes from an Element with jQuery
In the same way you can add classes to an element with jQuery's addClass() function, you can remove them with jQuery's removeClass() function.

Here's how you would do this for a specific button:

$("#target2").removeClass("btn-default");
Let's remove the btn-default class from all of our button elements.

## Change the CSS of an Element Using jQuery
We can also change the CSS of an HTML element directly with jQuery.

jQuery has a function called .css() that allows you to change the CSS of an element.

Here's how we would change its color to blue:

$("#target1").css("color", "blue");
This is slightly different from a normal CSS declaration, because the CSS property and its value are in quotes, and separated with a comma instead of a colon.

Delete your jQuery selectors, leaving an empty document ready function.

## Disable an Element Using jQuery
You can also change the non-CSS properties of HTML elements with jQuery. For example, you can disable buttons.

When you disable a button, it will become grayed-out and can no longer be clicked.

jQuery has a function called .prop() that allows you to adjust the properties of elements.

Here's how you would disable all buttons:

$("button").prop("disabled", true);
Disable only the target1 button.

## Change Text Inside an Element Using jQuery
Using jQuery, you can change the text between the start and end tags of an element. You can even change HTML markup.

jQuery has a function called .html() that lets you add HTML tags and text within an element. Any content previously within the element will be completely replaced with the content you provide using this function.

Here's how you would rewrite and emphasize the text of our heading:

$("h3").html("<em>jQuery Playground</em>");
jQuery also has a similar function called .text() that only alters text without adding tags. In other words, this function will not evaluate any HTML tags passed to it, but will instead treat it as the text you want to replace the existing content with.

Change the button with id target4 by emphasizing its text.

View our news article for <em> to learn the difference between <i> and <em> and their uses.

Note that while the <i> tag has traditionally been used to emphasize text, it has since been adopted for use as a tag for icons. The <em> tag is now widely accepted as the tag for emphasis. Either will work for this challenge.

## 
Select target1 and change its color to red.
## 
