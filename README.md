Download Link: https://assignmentchef.com/product/solved-cse-330-laboratory-3-and-homework-assignment-2
<br>
<strong style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">PART 1</strong>

<span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">Complete the ADT Vector implementation from our previous labs by adding the following two functions to the Vector class:</span>




<ol>

 <li>Member function void erase(int k){…} which removes the element at index k.</li>

</ol>




<ol start="2">

 <li>Member function void insert(int k, T x){…} which inserts the new element x at index k. (The element that is at index k prior to insertion and all other elements at higher-numbered indices are to move one position to the right.)</li>

</ol>







Details of the processes behind both functions are depicted below.




<strong>Erase:</strong>      Erase the element at index 3 in vector [2][4][6][<u>8</u>][10][12][14][16]




Step-by-step …

0   1   2   3    4     5     6    7

… [2][4][6][<u>8</u>][10][12][14][16]




… [2][4][6][10][10][12][14][16]




… [2][4][6][10][12][12][14][16]




… [2][4][6][10][12][14][14][16]




… [2][4][6][10][12][14][16][16]




… [2][4][6][10][12][14][16][<span style="text-decoration: line-through;">16]</span>




… [2][4][6][10][12][14][16]    DONE!




Look at the example and realize the kinds of shifts (really, “copies”) that will have the desired effect. Also notice the duplicate element at the end and how it is removed in order to produce the final result.




Your function should also handle the <u>special case</u> where the removal index is the index of the element at the highest index … what will be the simplest way to accomplish this element’s removal? (Hint: this function already exists).







<strong>Insert:</strong>      Insert new element 7  at index 3 in vector [2][4][6][<u>8</u>][10][12][14][16]




Step-by-step …

0   1   2   3    4     5     6    7

… [2][4][6][<u>8</u>][10][12][14][16]




… [2][4][6][8][10][12][14][16][<u>16</u>]




… [2][4][6][8][10][12][14][14][16]




… [2][4][6][8][10][12][12][14][16]




… [2][4][6][8][10][10][12][14][16]




… [2][4][6][8][8][10][12][14][16]




… [2][4][6][<u>7</u>][8][10][12][14][16]    DONE!







Look at the example and realize the kinds of shifts (really, “copies”) that will have the desired effect. Also notice how the process  starts out with the addition of a copy of the last element at the right of end of the vector.




Your function should also handle the <u>special case</u> where the insertion  index is the index that is one more than the highest index pre-insertion … what will be the simplest way to accomplish insertion into this index? (Hint: this function already exists)




<strong>Wait for instructions on how to test your erase and insert member functions …  </strong>

<strong> </strong>

<strong> </strong>

<strong>PART 2 </strong>

<strong> </strong>

Add to your Vector class two additional functions:




void erase(iterator itr){ …}     and    insert(iterator itr, T x) {…}




These two member functions are to erase the vector item referenced by iterator itr, and to insert at some iterator itr a new value x.<strong><em> It is expected that Part 2 will largely be accomplished as part of Homework 2.  </em></strong>




Again, await instructions on how to test these two iterator-based member functions.

<strong>  </strong>

<strong>For Lab Credit: </strong>Simply sign your name of the signup sheet. No portal submissions are required.

<strong> </strong>

<strong>For Homework Assignment 2: Submit on Wednesday, Jan 29, 2020, via the BlackBoard portal </strong> the following files:  (1) file Vector.h with both variants of your member functions erase and insert “highlighted” with lines

//**************** LAB3/HW2 start ************************************** … your four functions …




//**************** LAB3/HW2 end ***************************************




<ul>

 <li>a hardcopy of file VectorMainHW2 .cpp with <u>test code to be determined,</u></li>

 <li>a typescript or screen capture that shows your compiling and running of the program . In case you do not achieve a running program, still submit the source code you have along with a typescript/screenshot that shows your “attempt” to compile and the compiler errors you get.</li>

</ul>




The homework assignment is worth 20 points, 5 points per functions.


