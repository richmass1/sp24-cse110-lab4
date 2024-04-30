1. The bug is that the input from a text box is stored as a string by default, and so using the + operator concatenates the strings.
2. I would fix it by casting `num1` and `num2` to numbers.