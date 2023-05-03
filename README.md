Download Link: https://assignmentchef.com/product/solved-cs-570-programming-foundations-homework-assignment-4
<br>
<strong>Note:</strong> This and all assignments given in this course can be and must be solved using <strong>only</strong> the materials that have been discussed in class.  Do not look for alternative methods that have not been covered as part of this course.

<strong> </strong><strong>Program 1 (60 points): </strong>

Rangers at the Serengeti National Park are in need of a program to simulate the ecological balance between lion and gazelle populations. Gazelles eat from an unlimited supply of grass; lions eat gazelles. Lions are the only obstacle to increasing population growth for the gazelles. The population of lions increases as the population of gazelles increases.

You have been asked to write a program to calculate the populations of gazelles and lions over a 1000-day period with population counts displayed every 100 days only. The program must request from the user the initial numbers of gazelles and lions. The following formulas are to be used for calculating the day-to-day changes in the gazelle (G) and lion (L) populations:

<strong>G</strong><strong>Tomorrow</strong><strong> = (1 + a) ∙ G</strong><strong>Today</strong><strong> – c ∙ G</strong><strong>Today</strong><strong> ∙ L</strong><strong>Today</strong><strong> L</strong><strong>Tomorrow</strong><strong> = (1 – b) ∙ L</strong><strong>Today</strong><strong> + c ∙ d ∙ G</strong><strong>Today</strong><strong> ∙ L</strong><strong>Today</strong>




Where:

<ul>

 <li><strong>= 0.01</strong> Fractional increase in gazelle population without competition from                     lions</li>

 <li><strong>= 0.008</strong> Fractional decrease in lion population without gazelle to eat <strong>c = 0.00005</strong>  Likelihood that a lion will encounter and eat a gazelle <strong>d = 0.015</strong>     Fractional increase in lion population attributed to a devoured</li>

</ul>




Finally, as summary information, print the highest individual daily population number of lions and of gazelles and the corresponding average values over the 1000-day time period.




<strong><em>Program details: </em></strong>




The program should welcome the user and prompt the user for input data with clear understandable messaging. Add proper error handling for erroneous input (e.g. values less than one). Make sure the user gets an explanatory error message if the supplied input is invalid. In case of invalid input, the user should be asked to try again until the input provided is valid.




The number of iterations (1000 days) must be defined as a declared constant integer. Values for <strong>a</strong>, <strong>b</strong>, <strong>c</strong>, and <strong>d</strong> have to be defined as constant as well. Choose the proper data types.




The program must use a repetition structure that loops 1000 times. Within the loop, using today’s values for <strong>G</strong> and <strong>L</strong>, compute the corresponding tomorrow values for <strong>G</strong> and <strong>L</strong>. While it is impossible to have a portion of a gazelle or of a lion, use <strong><sub>double</sub></strong> data types for all <strong>G</strong> and <strong>L</strong> values anyway.




Use a selection structure to identify a 100th iteration, allowing displaying on the monitor the population values for that iteration.




Use selection structures to determine the highest number individual daily population of both lions and gazelles.




You also need to determine the overall sum of gazelles and lions (for calculating the average) over the 1000-day period to be displayed as summary information.




Summary information has to be printed to the output. Here is a sample run of a typical solution to this problem:




<strong>Note on formatting output to print the table: </strong>




In order to be able to display the table in a pleasant and easy to read format (e.g. population figures with 2 decimal places, the three columns under the headings and aligned to the left,  etc.) you may want to use either

<strong>System.out.printf()</strong> or <strong>System.out.format()</strong>methods of <strong>System.out</strong>.  These output methods allow you to specify formatting information for the objects to be displayed, such as the size of the printing field, the alignment

(left, right), and the number of decimal places after the decimal point

(among other things)




The first parameter in either one of these methods is a string that specifies the format.  The format is specified using converters and flags.  For example:







<strong>double pi = Math.PI; </strong>

<strong>System.out.format(“%-4s%10.3f%n”, “pi: ”, pi);    </strong>




will display <strong><sub>pi</sub></strong> as a number with 3 decimal places after the decimal point, using a printing field of size 10, aligned to the left:




<strong>pi:      3.142       </strong>




In this example:




<strong>%</strong><strong><sub>-4s</sub></strong> indicates that the object to be displayed is a string (<strong><sub>s</sub></strong>), that will be printed in a field of size <strong><sub>4</sub></strong>, aligned to the left (<strong><sub>–</sub></strong>) of the printing space.




<strong>%10.3f</strong> indicates that the object to be displayed is a floating-point number (<strong><sub>f</sub></strong>), that it should be displayed in field of size <strong><sub>10</sub></strong>, and with <strong><sub>3</sub></strong> decimal places after the decimal point.

<strong>%n</strong> is to advance to the next line after displaying <strong><sub>pi</sub></strong> (similar to <strong><sub>
</sub></strong>)

Converts commonly used include <strong><sub>f</sub></strong> for floating-point numbers, <strong><sub>s</sub></strong> for strings, <strong>n</strong> for new line.  Flags commonly used include <strong><sub>–</sub></strong> to align to the right.

You can find more information at:

<a href="https://docs.oracle.com/javase/tutorial/java/data/numberformat.html">https://docs.oracle.com/javase/tutorial/java/data/numberformat.html</a>




<strong>Program 2 (40 points): </strong>

Write a recursive method that:

<ul>

 <li>Receives a integer number <strong>n</strong> as its parameter</li>

 <li>Prints the out all the even numbers between <strong>n</strong> and <strong>0</strong> (inclusive)</li>

 <li>Returns the number of even number between <strong>0</strong> and <strong>n</strong>, for any positive integer <strong>n</strong></li>

</ul>

Make sure that you include a <strong>base case</strong>. What is the <strong>recursive case</strong>? Let the recursive case solve a simpler problem.




Test your recursive method in a <strong>main</strong> method that:

<ul>

 <li>Asks the user to enter a positive integer value, or 0 to end the program  Validates the user’s input: if the user enters a negative value, the program should issue an error message and ask the user to try again until a valid value is entered</li>

 <li>Calls the recursive method and prints the returned value</li>

 <li>Goes back to ask the user to enter a positive integer value, or 0 to end the program (<em>hint</em>: you need a loop)</li>

</ul>




<strong> </strong>

<strong>Note:  </strong>Please make sure to submit well-written programs for these programming tasks. Good identifier names, useful comments, indentation, and spacing will be some of the criteria that will be used when grading this assignment.




<strong> </strong>