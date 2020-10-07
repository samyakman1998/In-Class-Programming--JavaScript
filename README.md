# In-Class-Programming — JavaScript

~*25 min total*

This repository is your starting point for the assignment and includes the instructions below.

Link to your GitHub pages website: `https://github.com/NEU-DS-4200-F20-Staff/In-Class-Programming--JavaScript.git`

# Aim of the assignment
Build comfort with how to use git, GitHub Pages, JS, and HTML.

# Instructions 
1. Edit near the top of this `README.md` file to include a clickable hyperlink to the GitHub page website for your repo., replacing the `` `[insert your clickable hyperlink here]` `` code with your markdown. (Detailed instructions for GitHub pages [here](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Using_Github_pages).)

1. Edit the files to include the functionality described in [this tutorial on w3resource](https://www.w3resource.com/javascript-exercises/javascript-basic-exercise-10.php).

# Submission instructions  

1. Commit all your local code and push it to your remote GitHub Classroom-generated repository.

1. Submit the URL of **your GitHub Classroom-generated repository** to the [activity assignment on Canvas](https://northeastern.instructure.com/courses/18721/assignments/573840). **Do not submit a link to a personal repository. It must be within our class GitHub organization.** 

# Stretch goal
If you are done with the first goal, try to build a simple calculator with all numbers as buttons and operations as buttons too. [This article](https://medium.com/@ethanryan/lets-make-a-javascript-calculator-a81186cb912f) has some ideas you can use, but consider trying things out yourself. You likely won't be able to get the full thing working in class but it will help you get a hands on experience of working with HTML, CSS and Javascript.

# Additional information
JavaScript (JS) is a high-level, interpreted programming language for computers. It is often run in web browser applications to create things that work by themselves like a popup message or a live clock or counter. It is based on the ECMAScript (ES) standard, and modern browsers support at least ES6 and often ES2016+. In this activity the different features do not matter. You can see [ES2016+ feature support in this table](https://kangax.github.io/compat-table/es2016plus/).

In the HTML file there is the line:
```html
<input type='button' onClick='multiplyBy()' Value='Multiply' />
```
This states that we have an HTML input field here which is of a button type and the value `'Multiply'` ends up as the button's label. It also states that when you click the button, the browser is supposed to call the JavaScript function `multiplyBy()` which is defined in the corresponding JS file. We should write the action that is expected to occur in this function definition.

Function explanation:
```javascript
function multiplyBy(){
        num1 = document.getElementById('firstNumber').value;
        num2 = document.getElementById('secondNumber').value;
        document.getElementById('result').innerHTML = num1 * num2;
}
```

Function keyword states that `multiplyBy()` will be defined as follows. Here, it says grab the value of the element having ID=`'firstNumber'` and put it into a variable called `num1` and ID=`'secondNumber'` into `num2`. For more info on how this works see [CSS Selectors on w3schools](https://www.w3schools.com/cssref/css_selectors.asp).

Now, grab the element of the document object model (DOM) on the HTML page with ID='result' and set its innerHTML property. We will now calculate the value by multiplying `num1 * num2` and then put this value into ID=`'result'` by this statement:
`document.getElementById('result').innerHTML = num1 * num2;`

Some more examples of using innerHTML can be found [on w3schools](https://www.w3schools.com/jsref/prop_html_innerhtml.asp).

# Assignment Setup (For Instructors Only)

See https://github.com/NEU-DS-4200-F20-Staff/Assignment_Setup_Instructions.
