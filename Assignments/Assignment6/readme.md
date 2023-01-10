# Assignment 4
# Explanation of Bubbling
In the JavaScript section, we have assigned the html elements (p1 and c1) using the querySelector () function to the variable parent and child.
After that, we have created and included an event which is the click event to both div element and child button. Also created two functions that will help us to know the sequence order of the execution of the parent and child. It means if the child event is invoked first, "child is invoked" will be printed otherwise "parent is invoked" will get printed.
Thus, when the button is clicked, it will first print "child is invoked" which means that the function within the child event handler executes first. Then it moves to the invocation of the div parent function.

# Explanation of Capturing
Moving towards the JS code, initially, we have assigned the html element, i.e., the p1 id, to a variable parent using the querySelector () method and the same we have done with the c1 id where we have assigned it to a variable child.
Then we have used a click event and attached it to both the p1 div and c1 button. Also containing a function for printing the appropriate message on the console. It means if the child event is invoked first, then it will print the "Child is invoked" message on the console first, and if the parent event handler is invoked first, it will "Parent is invoked" message on the console first.
Next, we have added a third argument of addEventListner () to true in order to enable event capturing in the parent div.
When we click on the button, it first executes the function, which is attached in the parent div.
Afterward, the onclick () function of the button runs, and it is because of event capturing. Due to event capturing, the event of the parent element executes first, and then the event of the target element gets executed.
