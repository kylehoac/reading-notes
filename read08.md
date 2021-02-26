# Reading Notes 08

__*Comparison Operators : Evaluating Conditions*__

- Comparison operators can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be boolean

*==* - Is equal to
*!=* - Is not equal to
*===* - Strict equal to (Compares two values to check that the data type and value are the same)
*!==* - Strict not equal to (Compares two values to check that the data type and value are *not* the same)
*>* - Checks if the number on the left is greater than the number on the right
*<* - Checks if the number on the left is less than the number on the right
*>=* - Checks if the number on the left is greater than or equal to the number on the right
*<=* - Checks if the number on the left is less than or equal to the number on the right

__*Logical Operators*__

- Logical operators allows you to compare the results of more than one comparison operator

*&&* - Tests more than one condition. If both expressions evaluate to true then the expression will return true. If one of the expressions evaluates to false, then the expression will return false.
*||* - Tests at least one condition. If either expression evaluates to true, than the expression will be true, if both expressions evaluate to false, then the expression will be false
*!* - This operator takes a single boolean value and inverts it. EX: !(2 < 1). This expression was false without the !, however with it, it returns as true

- Logical expressions are evaluates left to right. If the first condition can provide information to get the answer, then there is no need to evaluate the second expression

__*Loops and Loop counters*__

- Loop checks a condition. If it returns true, a code block will run. It will then check a condition again, and if it still returns true, then the code block will run again. This will continue looping until the condition returns false.

Types of loops include:

- *for* - Used for if you need to run a code a specific number of times. The condition is usually a counter which is used to tell how many times to run a loop Ex: for (var i = 0; i < 10; i++>). This code would write 0123456789 on the page with a document.write(i) code following it.

- *while* - Used for if you dont know how many times the code should run. The code will loop for as long as the condition is true.

- *do while* - Similar to the *while* loop, however will always run statements inside of curly braces at least once, even if the condition is false.

A for loop uses a counter as a condition. The condition is made of the following 3 statements:

- initialization - Create a variable and set it to 0. The variable is commonly called *i*, or *index* and acts as a counter. ( var i = 0;)

- condition - The loop should continue to run until the counter reaches a certain number. (i < 10)

- update - every time the loop has run the statements in the curly braces, it adds one to the counter (i++) (can also use -- to count down)
