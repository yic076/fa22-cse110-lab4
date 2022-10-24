1. line 12 will print i to the console. In this case, it prints 3. This is because in the for loop, the loop stops once i is greater or equal to the length of prices. And since the length of prices is 3 (3 elements in the array), i is 3 when the loop terminates. And since i is decalred using var, it is visible through out the function. 
2. line 13 will print the discounted price before rounding (so it maybe possible to return a number with more than 2 digits in the decimal place) of the final element in prices. In this case it print 150. Only the final element's discounted price is returend becasue this line happened after the loop terminates. 
3. line 14 will print the rounded version of the discounted price and in this case print 150. Also only the final element's price is returned because this line is after the loop terminates. 
4. The function returns discuonted, which is a collection of all the finalPrice for each of the element passed in. In this case it will return `[50,100,150]`
5. This time line 12 will result an error, becasue i is defined using let and is no longer visible outside of the for loop. 
6. Similarly, discounted price result an error, it also isn't visible outside of the for loop since it's defined using let.
7. Line 1 still prints the rounded discounted price of the last element to the console. Although it's defined using let, it's defined in the function and not in the for loop, so line 14 can still see finalPrice.
8. Similarly, the function can still return the array `[50,100,150]` because discounted is defined in the function, and not in the loop. 
9. Line 11 results an error for the same reason as question 5, i isn't within the scope for line 11.
10. Line 12 will print 3 to the console becasue length is defined in the function, not in the loop.
11. This will acutally still return `[50,100,150]` because const means that a variable can't be assigned anymore using equal sign. But the push operation at line 8 isn't assigning discounted to a new value; it's modifiying, which is allowed. 
12. student.name
    student['grad year']
    student.greeting()
    student['favorite teacher'].name
    student.courseLoad[0]
13. A. result is 32 because integer 2 is mapped to its string representation.  
    B. result is 1 because `-` isn't an operator for string concatenation, so the string 3 here is convereted to the number 3 unlike the question A.  
    C. result is 3 because null is converted to 0 when adding to a number  
    D. result is 3null because null is converted to the string `null` when adding to a string
    E. result is 4 because true is converted to 1 when adding to a number  
    F. result is 0. Opposite to true, false is converted to 0 and so is null during an arthmetic operation. So it's 0 + 0 = 0  
    G. result is 3undfined. Similar to how string 3 + null is 3null, same conversion happened here. 
    H. result is undefined or NaN. Subtraction doesn't result in string due to the same reason in question B. So it's number 3 - undefined which is undefined  
14. A. Strings numbers are converted to numbers, so 2 is greater than 1 and is true
    B. In this case, since both 2 and 12 are strings, they can be compared properly without needing for any conversion. In this case, it's comparing the ascii value. And since 2 comes after the 1 from 12, 2 is actually greater than 12. So false
    C. True. == is regualar equality check which means type conversion is allowed. So string 2 is converted to numeric 2 and therefor they are equal.
    D. False. === is strict equality which means no type conversion. And there fore, a string is not the same as a number and returns false.
    E. False. True is converted into 1 during numeric comparison and 1 is not equal to 2.
    F. True. boolean(2) converts 2 into a boolean. And such a conversion makes any non 0 number into the boolean true. So true === true 
15. == is comparison that accepts conversion while === doesn't. So in ensence, == returns true even for different datatypes as long as they can be converted into equivalent values. But === requires the two objects to be of the same datatype and value or else it returns false.
17. Do something simply mutiplies a number by 2. Here on line 13, array [1,2,3] and the function do something is passed to modifyArray. In there, dosomething is stored in parameter callback. So as the loop is traversing through the element in the passed in array, each element is then passed to doSomething/callback and is mutiplied by 2. The result is then pushed into newArr. So the final returned array is [2,4,6]   
19. 1 4 3 2 are printed in this order. 1, 4 are printed out stright up (order determined by the line number) 3 has to go through setTimeout but since the delay is set to be 0, it appers to be instant but still falls behind 1 and 4. Then finally 2 is printed after 1 second.   
