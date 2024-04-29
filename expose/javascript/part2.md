1. The number 3 is logged to the console. The variable `i` is declared with `var` in a for loop header, so it persists after the for loop ends. The loop ends when `i` equals `prices.length`; in this case `prices.length` is 3, so `i` is 3 and 3 is logged.
2. 150 is logged. Since `discountedPrice` was declared with `val`, it persists after the for loop; its last value is (1-0.5)*300, which is 150.
3. 150 is logged. `finalPrice` gets its value from the last iteration of the for loop; where it is assigned 150 rounded to two decimal places, which is still 150.
4. It returns the list [50, 100, 150], because these are the values that were added to the array `discounted`, and the function returns `discounted`.
5. It will throw an error, because `i` is only defined in the scope of the for loop; this is a consequence of declaring `i` with `let`.
6. It will throw an error for the same reason as question 5.
7. It will log 150. Because `finalPrice` was declared outside the scope of the for loop, its value persists after the loop ends.
8. It will return the list [50, 100, 150] for the same reason as question 4.
9. It will throw an error, because `i` was declared with `let`, and so it does not persist after the for loop. `i` will be undefined when line 11 executes.
10. It will log 3, because line 12 is in the same scope as line 4 where `length` was declared and assigned the value 3.
11. It will return the list [50, 100, 150], because although `discounted` was declared with `const`, the method `push` is still able to modify the array that has the name `discounted`.
12. 
A. student.name
B. student['Grad Year']
C. student.greeting()
D. student['Favorite Teacher'].name
E. student.courseLoad[0]
13. 
A. '32', because it interprets 3 as a string
B. 1, because it interprets '3' as an int
C. 3, because it interprets null as 0
D. '3null' because it interprets null as the string 'null'
E. 4 because it interprets true as 1
F. 0 because false and null are both interpreted as 0
G. '3undefined' because undefined is interpreted as a string
H. NaN because undefined is interpreted as NaN when it's converted to a number
14. 
A. true, because '2' is converted to the number 2
B. false, because '2' and '12' are both strings, and '2' comes after '12' alphabetically (I use this term loosely)
C. true because '2' is converted to 2
D. false, because `===` returns false when the operands are of different types
E. false, because true is converted to 1
F. true, because casting 2 to boolean returns true, as with any other nonzero number
15. `==` tries to convert one of the operands so that they become the same type, and then compares them; `===` does not attempt to convert its operands, instead, it simply returns false when they are different types.
17. It will return the array [2, 4, 6]. It iterates through the array that's passed to it, [1, 2, 3], and calls `doSomething` on each value. `doSomething` returns each value multiplied by 2, and then these values are added to an array called `newArr`. Finally, it returns `newArr`.
19. It logs 1, pauses for 1 second, then logs 2, 3, and 4 (on separate lines)