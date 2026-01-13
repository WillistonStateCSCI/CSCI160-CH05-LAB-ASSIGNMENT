# CSCI160-CH05-LAB
About Programming Exercises From Java Illuminated Book by Anderson and Franceschi
## Q05_55 Instructions  
We want to build a simple "English language" calculator that does the following:  
* takes three inputs from the keyboard, two of them single digits (0 to 9)  
* takes a *char* from the keyboard, representing one of five operations from the keyboard: + (addition), - (subtraction), * (multiplication), / (division), and ^ (exponentiation)  
* outputs the description of the operation in plain English, as well as the numeric result  
  
For instance, if the two numbers are 5 and 3, and the operation is *, then the output should be "five multiplied by three is 15"  
Note that the result is given as a number, not a word.  
If the two numbers are 2 and 9, and the operation is -, then the output should be "two minus nine is -7"  
If the two numbers are 5 and 2, and the operation is ^, then the output should be "five to the power two is 25"  
Hint: to perform the exponentiation, use the *pow* method of the *Math* class.  
If the two numbers are 5 and 0, and the operation is /, then the output should be "Division by zero is not allowed"  
Here, the operation will not be performed.  If the two numbers are 25 and 3, and the operation is +, then the output should be "Invalid Number"  because 25 has two digits.  
As for the operators, they should be translated into English as follows:  
* \+ plus  
* \- minus  
* \* multiplied by  
* / divided by  
* ^ to the power  
  
You should use the *switch...case* selection statement to translate the input values into words.  
You need to consider these special situations:  
* For division, there is a special constraing:  you cannot divide by 0, and you should therefore test whether the second number is 0.  If it is 0, then you should output a message saying that you are not allowed to divide by 0.  
* The "operator" is not one of the preceding five operators;  In that case, output a message saying that the operator is not a valid one.  
* One or two of the numbers is not a valid digit; again, you should output a message to that effect.  
* Hint: You can deal with these special situations in the *default* statement of the *switch* block and possibly use some *boolean* variables to keep track of this information, as you may need it later in your program.  
### Q05_55 Test 1
**Input:**  
3  
5  
\*       
**Output:**  
three multiplied by five is 15  
### Q05_55 Test 2
**Input:**  
2  
9  
\-       
**Output:**  
two minus nine is -7  
### Q05_55 Test 3
**Input:**  
5  
2  
^       
**Output:**  
five to the power two is 25  
### Q05_55 Test 4
**Input:**  
6  
3  
/       
**Output:**  
six divided by three is 2  
### Q05_55 Test 5
**Input:**  
5  
0  
/       
**Output:**  
Division by zero is not allowed  
### Q05_55 Test 6
**Input:**  
5  
1  
&       
**Output:**  
Invalid operator   
### Q05_55 Test 7
**Input:**  
5  
25  
+       
**Output:**  
Invalid number     
