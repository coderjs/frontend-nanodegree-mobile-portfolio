### VIEW ONLINE:
This project can be viewed online here: [Mobile Portfolio Template](http://coderjs.github.io/frontend-nanodegree-mobile-portfolio/)

### PROJECT OBJECTIVES
This is my submission for project 4 of the Udacity Front End Developer Nanodegree program. The objective of this project is to optimize a provided website with a number of optimization- and performance-related issues so that it achieves a target PageSpeed score and runs at 60 frames per second (~16ms).

### PROJECT OUTCOME:
	Original File (http://cameronwp.github.io/udportfolio/views/pizza.html)
		* Time to generate pizzas on load: 14.64ms
		* Time to resize pizzas: 138.045ms
		* PageSpeed Insight Score - Root: 28/100 (http://cameronwp.github.io/udportfolio/)
		* PageSpeed Insight Score - Pizza: 66/100 (http://cameronwp.github.io/udportfolio/views/pizza.html)
		
	Optimized File :
		* Time to generate pizzas on load: 12.46ms
		* Time to resize pizzas: 1.72ms
		* PageSpeed Insight Score - Root: 91/100 (http://coderjs.github.io/frontend-nanodegree-mobile-portfolio/)
		* PageSpeed Insight Score - Pizza: 77/100 (http://coderjs.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html)

### APPROACH:
As I am still a relatively new developer (and these are relatively advanced concepts for me), I have approached this project as follows:
	1. Watched all specified Udacity course lectures and completed all quizes
	2. Reviewed many of the recommended Udacuty supplemental materials
	3. Conducted extensive independent research on core subject-matter to shore-up my comprehension (links referenced in file)
	4. Reviewed and reverse engineered the work of other [more advanced] students who have previously completed this project to better undertand the proper approach
		(for this project I have analyzed & benchmarked the posted work of github handles bw120, micyang, bahalps, jgroeder, kleinbottled, and others)

### CONCEPTS LEARNED AND APPLIED:
In this assignment I have learned and applied the following concepts:
	* Performance benefits of reducing [large] image size
	* Performance benefits of simplifying unnecessarily complex code
	* Performance benefits of eliminating forced layout
	* Performance benefits of preventing unnecessary looping through arrays of variables
	* Performance benefits of not painting objects that arent visible to the user on page speed
	* Benefits of employing User Timing APIs to measure performance of specific components
	* Performance comparison between querySelector() and getElementBy_()

### SUMMARY OF CHANGES:
Below is a partial summary of the changes made to this sample portfolio.
	* images
		1. I customized and minified the images according to specified requirements
	* html pages
		1. Referenced the smaller images in the html files
	* views/main.js
		1. Used getElementsByClassName() instead of querySelectorAll() and moved outside loop
		2. Fixed random bug (changed adjective "noise" to the intended "noisy")
		3. Replaced function determineDx() with simpler code
		4. Made minor changes to User Timing API
		5. Used style.transform instead of using style.left to change position
		6. Reduced number of pizza columns
		7. Moved mPizzas function outside of loop
		8. Reduced number of pizzas to display on page
	* views/css.style
		1. Added additional attributes to css classes, removing them from javascript
	* Other/Misc
		1. Linted javascript code
