Loops and conditional statements are fundamental constructs in MATLAB that allow you to control the flow of your program. Here's a guide on how to use loops and conditional statements:

### Conditional Statements (if, else, elseif):

1. **if Statement:**
   - Use the `if` statement to execute a block of code when a condition is true.

   ```matlab
   % Example if statement
   x = 10;

   if x > 5
       disp('x is greater than 5');
   end
   ```

2. **if-else Statement:**
   - Use the `else` statement to execute a block of code when the condition in the `if` statement is false.

   ```matlab
   % Example if-else statement
   y = 3;

   if y > 5
       disp('y is greater than 5');
   else
       disp('y is not greater than 5');
   end
   ```

3. **elseif Statement:**
   - Use `elseif` to check additional conditions if the previous ones are false.

   ```matlab
   % Example elseif statement
   z = 7;

   if z > 10
       disp('z is greater than 10');
   elseif z > 5
       disp('z is greater than 5 but not 10');
   else
       disp('z is 5 or less');
   end
   ```

### Loops (for, while):

1. **for Loop:**
   - Use the `for` loop to iterate a fixed number of times.

   ```matlab
   % Example for loop
   for i = 1:5
       disp(i);
   end
   ```

2. **while Loop:**
   - Use the `while` loop to iterate as long as a condition is true.

   ```matlab
   % Example while loop
   counter = 1;

   while counter <= 5
       disp(counter);
       counter = counter + 1;
   end
   ```

3. **break Statement:**
   - Use `break` to exit a loop prematurely.

   ```matlab
   % Example break statement
   for i = 1:10
       disp(i);

       if i == 5
           break;
       end
   end
   ```

4. **continue Statement:**
   - Use `continue` to skip the rest of the loop's code and move to the next iteration.

   ```matlab
   % Example continue statement
   for i = 1:5
       if i == 3
           continue;
       end
       disp(i);
   end
   ```

5. **Nested Loops:**
   - You can nest loops inside each other.

   ```matlab
   % Example nested loops
   for i = 1:3
       for j = 1:2
           disp([i, j]);
       end
   end
   ```

These examples cover the basics of using conditional statements and loops in MATLAB. They are powerful tools for controlling program flow and iterating over data. Experiment with different conditions and loop structures to gain a better understanding of their behavior.
