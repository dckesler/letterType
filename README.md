letterType
==========

An angular directive that will make a message appear one letter at a time, and when done the message fades out.

---------

###Documentation

The directive is called letterIn, and is an attribute for an element.
The scope of the directive takes in 4 variables.
* word - the message that will be displayed; required,
* wait - how long in milliseconds before the message is displayed; the default is 0,
* speed - how many milliseconds inbetween letters appearing; the default is 200,
* fade - how many milliseconds it takes the message to fade away; the default is 1000; 'never' will make it so the word never fades out.

###Example

`<p letter-in word="Type this out" wait="5000" speed="400" fade="2000"></p>`

Here the message "Type this out" would come in after 5000 milliseconds, the letters would come in every 400 milliseconds, and after the message has loaded it would take 2000 milliseconds to fade away.

`<p letter-in word="Hello World" fade="never">`

Here the message Hello World will come in on page load, the letters come every 200 milliseconds, after the message has loaded it will never fade out.
