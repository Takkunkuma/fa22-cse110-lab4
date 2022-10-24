### The answers to the questions for Part 2.
<ul> 
    <li>Question 1. What will happen at line 12 and why? If the code causes an error, explain why. </li>
    <ul>
        <li> Answer: Will print 2 to the console. This is because the var declared i will increment in the for loop. Additionally, since var has a functional scope, the variable can be accessed anywhere as long as it is within the function. </li>
    </ul>
    <li>Question 2. What will happen at line 13 and why? If the code causes an error, explain why. </li>
    <ul>
        <li>Answer: This will print 150 onto the console, the reasoning is veru similar to Question 1 where the discounted price will save info for the last price that is discounted and can be accessed everywhere within the function.</li>
    </ul>
    <li>Question 3. What will happen at line 14 and why? If the code causes an error, explain why. </li>
    <ul>
        <li>Answer: This will print 150 onto the console, the variable is in a functional scope and the rounding of * 100 is a whole number which will also be a whole number after being divided by 100.</li>
    </ul>
    <li>Question 4. What will this function return? Give a brief explanation why. If the code causes an error, explain why. </li>
    <ul>
        <li>Answer: This function will return an array with all the discounted price which are [50, 100, 150]. The array discounted has a functional scope which can be accessed until return. </li>
    </ul>
    <li>Question 5. What will happen at line 12 and why?  If the code causes an error, explain why. (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5)).</li>
    <ul>
        <li>Answer: This will cause an error for undefined variable. Let keyword has a block scope, so the declaration for let will stay within the block of for loop. This can not be accessed outside of the for loop so the compiler will not recognize the variable i. </li>
    </ul>
    <li>uestion 6. What will happen at line 13 and why? If the code causes an error, explain why.</li>
    <ul>
        <li>Answer: Similar to Question 5, the variable discountedPrice is declared as a let variable, within the for loop, this means that the variable can only be accessed within the for loop. So this line will cause an undefined variable error.  </li>
    </ul>
    <li>Question 7. What will happen at line 14 and why? If the code causes an error, explain why.</li>
    <ul>
        <li>Answer: the final price variable has a scope within the function so it can be accessed anywhere, thus it will print out the last  dicounted price which is 150. </li>
    </ul>
    <li>Question 8. What will this function return? Give a brief explanation. If the code causes an error, explain why.</li>
    <ul>
        <li>Answer: This will return [50,100,150], which the return variable of discounted can be accessed everywhere within the function.  </li>
    </ul>
    <li>Question 9. What will happen at line 11 and why? If the code causes an error, explain why.</li>
    <ul>
        <li>Answer: This will cause an undefined variable error. The variable i has keyword let, which stays within the scope of the for loop as it has block scope. </li>
    </ul>
    <li>Question 10. What will happen at line 12 and why? If the code causes an error, explain why.</li>
    <ul>
        <li>Answer: This will print out length as 3. This variable with keyword const has a block scope and since console.log is being called within the same curly braces, line 12 would be able to access the variable. Moreover, there is no variable reassignment so it obeys all the requirements characteristics for const keyword.</li>
    </ul>
    <li>Question 11. What will this function return? Give a brief explanation. If the code causes an error, explain why.</li>
    <ul>
        <li>Answer: The return statement will return the array of discounted price. Const keywords don't allow for reassignment, however using methods to apply changes to the data type is allowed.</li>
    </ul>
</ul>

### Datatypes
<ul>
<li>Question 12. </li>
    <ul>
        <li>Accessing the value of the name property in the student object: student.name</li>
        <li>Accessing the value of the Grad Year property in the student object: student["Grad Year"] </li>
        <li>Calling the function for the greeting property in the student object: student.greeting()</li>
        <li>Accessing the name property of the object in the Favorite Teacher property in student: student["Favorite Teacher"].name</li>
        <li>Access index zero in the array of the courseLoad property of the student object: student.courseLoad[0]</li>
    </ul>
</ul>

### Basic Operators & Type Conversion 
13. Arithmetic
<ul>
<li>‘3’ + 2 = 32, using addition operator to string would convert number to string and performs string concatenation.</li>
<li>‘3’ - 2 = 1, using `-` will turn string into number and performs arithmetic subtraction. </li>
<li>3 + null = 3, null will be interpreted as 0 in number arithmatic. </li>
<li>‘3’ + null = 3null, null will be interpreted as string in string concatenation. </li>
<li>true + 3 = 4, true will be interpreted as 1 in number arithmatic. </li>
<li>false + null = 0, both of the values are interpreted as 0 as no string types are specified. Then arithmatic operation is performed.</li>
<li>'3' + undefined = 3undefined, the variable undefined is interpreted as a string and will perform string concatenation.</li>
<li>'3' - undefined = NaN, undefined keyword in number is defined as NaN, performing addition on NaN will leave another NaN.</li>
</ul>

14. Comparison
<ul>
<li>‘2’ > 1, this will return true because 2 will be interpreted as number. </li>
<li>‘2’ < ‘12’, this will return false because in alphabetical order, 1 would be smaller than 2. </li>
<li>2 == ‘2’, this will return true, the string becomes a number, and 2 == 2. </li>
<li>2 === ‘2’, this returns false because === does strict comparison which interprets variables without type conversions. </li>
<li>true == 2, false because true is 1 and 1 != 2. </li>
<li>true === Boolean(2), true, because boolean(2) will return true as number input into Boolean will return true. Since left and right side of === both have boolean data type, comparison returns true. </li>
</ul>   

15.  Explain the difference between the == and === operators.
<ul>
<li>The === operator is strict non-equality where the data type and value are both compared. The == operator is non-strict where depending on the way it's written, it may convert the data type first then perform data value comparison.</li>
</ul>

17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result. (This should be in your part2.md). Here we are passing in a function as a parameter, however we can also return a function from another function just as easily, you're encouraged to play around with callbacks as they are used heavily in frontend JS development. 
<ul>
<li>
This function will return an array: [2,4,6]. After modifyArray is called, the array parameter will have array [1,2,3] and callback will hold the function doSomething. In the forloop, the content returned by callback will be pushed into newArr as entries of list. doSomething will return twice the input. Thus the returning array after the execution of modifyArray will be [2,4,6]
</li>
</ul>

19. What is the output of the above code?
<ul>
<li>
1, 4, 3, 2.
</li>
</ul>