Download Link: https://assignmentchef.com/product/solved-cmis-102-hands-on-lab
<br>
<strong>Overview:</strong>

This hands-on lab allows you to follow and experiment with the critical steps of developing a program including the program description, Analysis, Design(program design, pseudocode), Test Plan, and implementation with C code. The example provided uses sequential, repetition, selection statements and two user-defined function.

<strong>Program Description:</strong>

This program will provide options for a user to calculate the square or cube of a positive Integer input by a user. The program will prompt the user to enter an Integer and then prompt the user if they want to calculate the square of the cube of the number. Based on the inputs of the user, the program will output the square of the cube of the positive integer. The program will then print the Integer and square or cube of the integer based on the user’s original choice. The program will continue to prompt the user for

Integers and their calculation choice until the user enters a negative integer. The square and cube calculations should be calculated using a function.

<strong>Analysis:</strong>

I will use sequential, selection, and repetition programming statements and functions for the cube and square calculations.

I will define three Integer variables: IntValue, MenuSelect, Results to store the Integer value input by the user, the Menu selection (1 for Square, 2 for Cube) of the user, and the results of the Square or Cube functions.

The Square function will take one Integer as input and return one Integer as the output. The calculation within the Square function is: Results = IntValue * IntValue

For example, if 10 was entered as the IntValue. Results = 10*10 = 100

The Cube function will take one Integer as input and return one Integer as the output. The calculation within the Cube function is: Results = IntValue * IntValue*IntValue

For example, if 10 was entered as the IntValue. Results = 10*10*10 = 1000

A repetition loop can be used to loop through iterations until a negative is entered: while(intValue &gt; 0) (




<strong>Program Design:</strong>




Main




<ul>

 <li>This program will provide options for a user to calculate the square</li>

</ul>




<ul>

 <li>or cube of a positive Integer input by a user.</li>

</ul>




<ul>

 <li>Declare variables</li>

</ul>




<ul>

 <li>Initialize loop variable intValue to positive value to start loop</li>

</ul>




<ul>

 <li>Loop While input is a positive number</li>

</ul>




//Prompt user for a number //Get user response




// Only perform menu and function calls if integer is positive If intValue &gt; 0 Then




//Prompt user for selection Square or Cube




// “Enter 1 to calculate Square, 2 to Calculate Cube ” If menuSelect == 1 Then




// Call the Square Function //Print results




Else If menuSelect == 2 Then // Call the Cube function //Print results




Else




//Print Invalid msg




End If //End of If menuSelect End If //End of If intValue &gt; 0




//END While




End // End of Main program




<ul>

 <li>Square Function ——————————</li>

</ul>

//Calculates the square of an Integer




<ul>

 <li>Cube Function ——————————</li>

</ul>

//Calculates the cubeof an Integer




<strong>Test Plan:</strong>




To verify this program is working properly the input values could be used for testing:




<table>

 <tbody>

  <tr>

   <td width="209">Test Case</td>

   <td width="208">Input</td>

   <td width="208">Expected Output</td>

  </tr>

  <tr>

   <td width="209">1</td>

   <td width="208">IntValue=10</td>

   <td width="208">Square of 10 is 100</td>

  </tr>

  <tr>

   <td width="209"></td>

   <td width="208">MenuSelect=1</td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="209">2</td>

   <td width="208">IntValue=10</td>

   <td width="208">Cube of 10 is 1000</td>

  </tr>

  <tr>

   <td width="209"></td>

   <td width="208">MenuSelect=2</td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="209">3</td>

   <td width="208">intValue=-1</td>

   <td width="208">Program exits</td>

  </tr>

 </tbody>

</table>













2




MenuSelect=N/A




<strong>Pseudocode:</strong>




Main




<ul>

 <li>This program will provide options for a user to calculate the square</li>

</ul>




<ul>

 <li>or cube of a positive Integer input by a user.</li>

</ul>




<ul>

 <li>Declare variables</li>

</ul>




Declare intValue, menuSelect,Results as Integer




// Set intValue to positive value to start loop Set intVal = 1;




// Loop While input is a positive number




While intValue &gt; 0




//Prompt user for a number




Print “Enter a positive Integer , Enter -1 to exit::”




Input intValue




// Only perform menu and function calls if integer is positive If intValue &gt; 0 Then




//Prompt user for selection Square or Cube




Print “Enter 1 to calculate Square, 2 to Calculate Cube: ” Input menuSelect




If menuSelect == 1  Then




// Call the Square Function Set Results = Square(intValue)




Print (“The sqaure of “ + intValue )




Print (“ is: “ + Results + &lt;NL&gt;)




Else If menuSelect == 2 Then // Call the Cube function set Results = Cube(intValue)




Print (The cube of “ + intValue )




Print (“ is: “ + Results +&lt;NL&gt;)




Else




Print “Invalid menu item, only 1 or 2 is accepted”




End If //End of If menuSelect End If //End of If intValue &gt; 0




END While




End // End of Main program













3




// Square Function ——————————




Function Square(Integer value) as Integer




//This function calculates the square of an integer //Input: value




//Output: Square




Set Square = value*value Return (Square)

End Function




// Cube Function ——————————




Function Cube(Integer value) as Integer




//This function calculates the cube of an integer //Input: value




//Output: Cube




Set Cube = value*value*value Return (Cube)




End Function







<strong>C Code</strong>




The following is the C Code that will compile in execute in the online compilers.




<ul>

 <li>C code</li>

</ul>




<ul>

 <li>This program will provide options for a user to calculate the square</li>

</ul>




<ul>

 <li>or cube of a positive Integer input by a user.</li>

</ul>




<ul>

 <li>Developer: Faculty CMIS102</li>

</ul>




<ul>

 <li>Date: Jan 31, 2014</li>

</ul>







#include &lt;stdio.h&gt;




<ul>

 <li>— the newer C compilers require that functions be prototyped</li>

</ul>




<ul>

 <li>— this tells the compiler what the input and output datatypes of the functions are</li>

</ul>




<ul>

 <li>— the functions are later defined after the main.</li>

 <li>function prototypes</li>

</ul>




int Square ( int ); int Cube ( int );




int main ()




{

/* variable definition: */




int intValue, menuSelect, Results; intValue = 1;




// While a positive number while (intValue &gt; 0)













4




{




printf (“Enter a positive Integer, Enter 0 or neg. no. to exit 
: “); scanf(“%d”, &amp;intValue);




if (intValue &gt; 0)




{




printf (“Enter 1 to calculate Square, 2 to Calculate Cube 
: “); scanf(“%d”, &amp;menuSelect);




if (menuSelect == 1)




{




// Call the Square Function Results = Square(intValue);




printf(“Square of %d is %d
”,intValue,Results);




}




else if (menuSelect == 2)




{




// Call the Cube function Results = Cube(intValue);




printf(“Cube of %d is %d
”,intValue,Results);

}




else

printf(“Invalid menu item, only 1 or 2 is accepted
”);




} //End If (intValue &gt;0) } //End WHile




return 0;




} //end of main /*********************************************/ /* function returning the Square of a number */

int Square(int value)

{

return value*value;

}




/* function returning the Cube of a number */ int Cube(int value)

{




return value*value*value;

}




Setting up the code and the input parameters in ideone.com:




Note the Input values for this run were: 10 1 10 2 -99

You can change these values to any valid integer values to match your test cases.

sults from running the programming at ideone.com:




<strong>ning Exercises for you to try:</strong>




<ol>

 <li>Modify the original code and using the Square and Cube functions as models, create a new function named Divide2 that would take an Integer input and returns a Float value of the input Integer divided by 2? Note this should be a float function. Take care when you prototype youir function. Add this as menu option 3 to the program to execute this function. Also include in menu option 3, the display of the results from this function. Make you have the datatypes correct for your variables. Support your experimentation with screen captures of executing the new code.</li>

</ol>




<ol start="2">

 <li>Modify the original code and create a new function of your own choice. This function should be unique and something you created for this assignment. Add this as menu option 4 to the program to execute this function. Your new function should have at least one argument input and return a calculated value to the main. You should also in the main display that returning value. Support your experimentation with screen captures of executing the new code. Make sure your datatypes of the variables/function are correct. <strong>Submit code as a separate .txt (or .c )</strong> <strong>file that includes all four menu options.</strong></li>

</ol>

<strong> </strong>

<ol start="3">

 <li>Prepare a new test table with at least 3 distinct test cases listing input and expected output for the code you created after step 2.</li>

</ol>




<ol start="4">

 <li>What would happen if we didn’t have the following test condition. I.e remove the following code from our design?</li>

</ol>




If intValue &gt; 0 {

} //End IF intValue &gt; 0




What happens if you entered a 0 for the menuSelect variable?




(Hint: You can try in the C code, or walk through it in the Pseudocode to see what happens.)








