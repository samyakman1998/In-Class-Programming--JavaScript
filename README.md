# In-Class-Programming--JavaScript

~*25 min total*

This repository is your starting point for the assignment and includes the instructions below.

Link to GitHub pages website: `[insert your hyperlink here]`

## Aim of the assignment
Build comfort with how to use git, GitHub Pages, JS, and HTML.

## Instructions 
Edit the files to include the functionality described in [this tutorial on w3resource](https://www.w3resource.com/javascript-exercises/javascript-basic-exercise-10.php).

## Submission instructions  
Modify the  `[insert your hyperlink here]` code in `README.md` to point to your GitHub pages URL. (Detailed instructions for GitHub pages [here](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Using_Github_pages).)
Commit your changes to your local repo and push to the remote GitHub repo.
Submit the URL of your repo to the [activity assignment on Canvas](https://northeastern.instructure.com/courses/18721/assignments/573840).

## Stretch goal
If you are done with the first goal, try to build a simple calculator with all numbers as buttons and operations as buttons too. [This article](https://medium.com/@ethanryan/lets-make-a-javascript-calculator-a81186cb912f) has some ideas you can use, but consider trying things out yourself. You likely won't be able to get the full thing working in class but it will help you get a hands on experience of working with HTML, CSS and Javascript.

## Additional information
JavaScript (JS) is a high-level, interpreted programming language for computers. It is often run in web browser applications to create things that work by themselves like a popup message or a live clock or counter. It is based on the ECMAScript (ES) standard, and modern browsers support at least ES6 and often ES2016+. In this activity the different features do not matter. You can see [ES2016+ feature support in this table](https://kangax.github.io/compat-table/es2016plus/).

In the HTML file there is the line:
```html
<input type="button" onClick="multiplyBy()" Value="Multiply" />
```
This states that we have an HTML input field here which is of a button type and the value `"Multiply"` ends up as the button's label. It also states that when you click the button, the browser is supposed to call the JavaScript function `multiplyBy()` which is defined in the corresponding JS file. We should write the action that is expected to occur in this function definition.

Function explanation:
```javascript
function multiplyBy(){
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result").innerHTML = num1 * num2;
}
```

Function keyword states that `multiplyBy()` will be defined as follows. Here, it says grab the value of the element having ID=`"firstNumber"` and put it into a variable called `num1` and ID=`"secondNumber"` into `num2`. For more info on how this works see [CSS Selectors on w3schools](https://www.w3schools.com/cssref/css_selectors.asp).

Now, grab the element of the document object model (DOM) on the HTML page with ID="result" and set its innerHTML property. We will now calculate the value by multiplying `num1 * num2` and then put this value into ID=`"result"` by this statement:
`document.getElementById("result").innerHTML = num1 * num2;`

Some more examples of using innerHTML can be found [on w3schools](https://www.w3schools.com/jsref/prop_html_innerhtml.asp).

## Assignment Setup (For Instructors Only):

### Create Repo

1. Go to this year's staff GitHub organization.

1. Create the new repository using a meaningful name.

1. Clone the repository locally.

1. Copy in the files from last year and make any necessary updates, *including assignment links to Canvas.*

1. Commit and push changes.

### GitHub Pages

It is necessary if using GitHub Classroom to set up GitHub pages for the students, as they do not have admin permissions on their repository. To do this, we need to create and move everything to the `gh-pages` branch and delete the `master` branch.

1. Commit the files to the `master` branch on GitHub.

1. `git branch gh-pages`

1. `git checkout gh-pages`

1. `git branch -D master`

1. `git push origin gh-pages`

1. On GitHub, go to `Settings`->`Branches` and set the default branch to `gh-pages`.

1. `git push origin :master`

### Template Repository

1. On GitHub, go to `Settings` and check the box for `Template repository` at the top. This makes GitHub Classroom copies much faster.

### GitHub Classroom

1. Create the assignment on GitHub Classroom.

1. Set the assignment title to be the same as on Canvas.

1. Set the deadline (23:59 of that day for in-class activities) and make sure it matches the assignment on Canvas.

1. Make the repository Public.

1. Set the template repository (where this file is) as the starter code.

1. Enable feedback pull requests.

1. Update assignment.

1. Enable the assignment invitation URL.

1. In the Canvas assignment, replace the old assignment invitation URL and template repo link URLs with the new ones.