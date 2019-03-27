# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment

**Huangyi Li (lhuangyi)**
* Chenhao Xu (chhaoxu)
* Huangyi Li (lhuangyi)
* Xinchen Rao (xrao)
* Li Zhu (izhuli)
* Cong Peng (Congp)

## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**
```js
	Example of a code comment:
	
	// Much code here provided by Colleen Van Lent, edited by Jackie Cohen -- and soon yourself
	// It is possible you have seen this before -- if so, that's fine, if not, that's fine, too

	// Output..

	// URI means something like URL -- slight differences for specificity

	// One place to find color option codes: https://www.w3schools.com/colors/colors_picker.asp

	//When someone uses the keyboard shortcut to copy the words "University of Michigan" then add the words "Go Blue" to the final div.  Each occurence should be on a separate line.
	//Note that this code must be outside the other function above
```
The characters I have to put before a comment is "//".

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

The tag ` <script> </script> ` tells the browser that I am running a Javascript program. The first function, alert, runs when the file is open in the browser. Then the second function and the third funtion, console.log and displayInformation, run after I click 'ok' on the pop-up window. The information printed with console.log can be seen in console. The fourth and the fifth funtion run after the program receives the action of user to copy text or click the button.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**

One is console.log and the other is alert.
I prefer to use console.log because I need to hit 'ok' to close the pop-up window of alert. In this way, it doesn't affect the use even though the developer forgets to remove it from debugging enviornment. Besides, console.log can show the object with values, where alert requires the developer to traverse the object first.

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**

```js
I have to comment the following code:
	alert("hello");
```

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**

Change the code `document.querySelector('h1').innerHTML = "A name";` in `function displayInformation ()` to `document.querySelector('h1').innerHTML = "Huangyi Li";`.


* **What does the word `document` represent in this code? Explain briefly.**

The global object "document" represents the HTML document which is displayed in the current browser window.
When html document is loaded in the browser, it becomes a document object. It is the root element that represents the html document. It has properties and methods. By the help of document object, we can add dynamic content to the web page.

* **What is happening in line 12 (`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**

The querySelector( ) method returns the first child element that matches a specified CSS selector(s) of an element while the getElementsByTagName( ) method returns a collection of all elements in the document with the specified tag name' li ' and the length property determines the number of elements with the specified tag name. So this commend returns the number of list items for this page when matching the id "items".

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

It would be white without any other colors.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**

For the border, we set the color of the border by 'border: 3px solid #FFFFFF'. I changed the background code to 'background-color: #0000ff' to get blue one.

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

We can find that the main part of this is the copyfunction.I replaced the 'Go Blue' with 'O Canada' and accordingly change the name of university in line 67, which determining the object we copy.

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
The original code declares a "function" named "handleClick()."
When the "function" is called, a "function alert()" runs and you will see a text box written "hello".

**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```
This part of code creates a button named "Wow" and when clicks the button "Wow", the "function handleClick()" will be called.
Once the "function" handleClick is called, you will see a text box written "hello".

* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

Based on the previous knowledge, I add 2 lines to relize this, firstly I add one line:
```js
 <input type="button" onclick="myFunction()" value="Spring Equinox 2019">  
 ```
 it can create a "Spring Equinox 2019" button and relate this button to a click incident.
 Then I add one line:
 ```js
 myFunction(){alert("March 20, 2019");}
 ```
 it creates a function to define the onclick incident.


### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

The code in `<style></style>` defines this.

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

We define a variable named 'regex' that will check if a string contains only characters between a-z and A-Z with any arrangement. ' [a-zA-Z] ' matches a single character, ' + ' means "one or more", so ' [a-zA-Z]+ ' matches one or more of those characters. '^' is the start  and '$' is the end.
I googled `var regex = /^[a-zA-Z]+$/;` and learned that it means variable regex matches any string of one or more letters and nothing else.(cite:https://www.sitepoint.com/expressions-javascript/).

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

In Javascript:
```js
if (condition){
	code
}
else {
	code
}
```
In python:
```js
if (condition):
	code
else:
	code
```
* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

That means the speed from showing up to disappearance. In this case, it is 10000 millisecond.

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```js
$(document).ready(function(){
```

Usually, every jQuery code begins with $(document).ready().
The ready() method is used to make a "function" available after the document is loaded.
(cite:https://www.w3schools.com/jquery/event_ready.asp)
Whatever code you write inside the $(document ).ready() method will run once the page DOM is ready to execute JavaScript code.

```js
$("form").submit(function(event){
```
The submit event occurs when a form is submitted. This event can only be used on form elements.
The submit() method triggers the submit event, or attaches a "function" to run when a submit event occurs.
(cite:https://www.w3schools.com/jquery/event_submit.asp)


* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.

I changed the line in the code below from `Nice!` to `Hello to you too!`.
```js
$("#result").html('<p class="good">Hello to you too!</p>').show().fadeOut(10000);
```
