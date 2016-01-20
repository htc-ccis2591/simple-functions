# HW2 - Simple Functions

## Goals
- Make functions in JavaScript that take input parameters
- Call functions and use return values
- Use JavaScript to get a value from a form field
- Use JavaScript to set a value from a form field
- Use String properties and methods


## Reading
Before you begin this assignment, you should read through chapter 3 in your textbook.

## GitHub Info
Repository:  https://github.com/htc-ccis2591/basic-functions

You need to fork this repository and submit a pull request to turn in the assignment.  Note that you also need to submit screenshots as described below to the D2L dropbox.

## Provided Files
Open the project (the basic-javascript folder) in Brackets. When using Brackets, it is important to open the entire folder, not just a single file.

Look at the index.html and script.js files provided.  


### Open and Run
Use the Brackets Live Preview feature to view the web page.  The page will show a series of forms that allow you to do some nifty things.  Click on one of the buttons.  Initially clicking the buttons will not appear to do anything.  Open the Developer Tools and go to the JavaScript Console and you will see some errors.
![Screenshot of initial JavaScript output and error](img/initial-output.png)

Important:  When a JavaScript syntax error is found, the browser will stop running the file. This is important to remember!


### JavaScript for the Form
Open the js/script.js file.  To complete the assignment, you will need to add JavaScript code as indicated in the comments. Before you begin, scroll down and look at the provided code that indicates it should not be modified.

This code is setup to handle working with the HTML form for you.  We haven't discussed most of what this code is doing, so examples are provided to get a nice functional form as well as for you to learn from.

#### Form Field values
We are getting the data to pass into our functions from the forms on the HTML page.  To get a form field value, we are using the id attribute of the form field to get that element from the DOM.  Then we get it's value property.

For example:
```JavaScript
   var earthWeight = document.getElementById("weight").value;
```

We can use similar syntax to set a value:
```JavaScript
   document.getElementById("moon-weight").value = "";
```

#### Event Listeners
We will discuss event listeners later in the course, but you'll see them in action here. In this assignment, they are used to do something when an event happens. Two events are used in this code.  

1. The focus event occurs when you click into an input field.  When that event occurs, the output field (and in some case other input fields) value is cleared out by setting it to the empty string.

2. The click event is used to say what happens when a button is clicked. Don't worry too much about the event handler right now, but pay attention to the code inside the function.  This will get the form input field value(s) and call the function you write to get the output. It then updates the form output field.  


## Assignment
The main focus of your assignment is to write the 4 functions that are used by the button click handlers:

1. Moon Weight
2. Dog Human Age
3. A Mini Calculator
4. String Length

The comments at the top of the JavaScript file provide information on how to write the functions.  Most of these are very basic, so don't over think it.  The Mini Calculator is a bit more involved, but still pretty straightforward.

Problem 4 also asks you to fill in the setup code.  Use the examples provided for problems 1-3 and setup problem 4 following the same pattern. This is intended to have you think about what that code is doing.

### Screenshots
You will also need to put two screenshots in the dropbox.  

1. For the first screenshot, you need to open the developer tools and go to your JavaScript source. Set a breakpoint inside of the calculateMoonWeight function and take a screenshot that shows the debugger paused at that line.  Notice that this allows you to see the value of your input parameter.
2. The second screenshot should be the output from the JavaScript console when the assignment is completed.


## Final Testing
When you are done, push your files to GitHub, then make sure that your page displays and runs correctly on the GitHub website.  

1. Go to your repository settings, and locate the URL where the page is published.  Copy this URL and use it as the website part of  the repository description.
2. Click the link to view the page and make sure that it runs correctly.  

After you have verified the page is working, create the pull request to submit the assignment.  Optionally, add a screenshot of your Open Pull Request to the assignment dropbox as well.
