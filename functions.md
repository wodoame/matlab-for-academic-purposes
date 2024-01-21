In MATLAB, functions are an essential part of programming, allowing you to organize and reuse code. Here's a guide on how to use functions in MATLAB:

### Creating a Function:

1. **Function Definition:**
   - Create a new script file or use the MATLAB editor to define your function. The file should have the same name as the function, with a `.m` extension.

   Example: Create a function named `myAddition` that adds two numbers.

   ```matlab
   % myAddition.m
   function result = myAddition(a, b)
       result = a + b;
   end
   ```

2. **Function Inputs and Outputs:**
   - Specify input and output parameters in the function definition.

   Example: The `myAddition` function takes two inputs (`a` and `b`) and returns the result.

### Using a Function:

1. **Calling the Function:**
   - Call the function by its name and pass the required arguments.

   ```matlab
   % Calling the function
   result = myAddition(3, 4);
   disp(result); % Displays 7
   ```

2. **Storing Function Output:**
   - You can store the output of a function in a variable.

   ```matlab
   % Storing the result
   myResult = myAddition(5, 2);
   ```

3. **Functions with Multiple Outputs:**
   - Functions can return multiple outputs.

   Example: Modify `myAddition` to return both the sum and the difference.

   ```matlab
   % myOperations.m
   function [sumResult, diffResult] = myOperations(a, b)
       sumResult = a + b;
       diffResult = a - b;
   end
   ```

   ```matlab
   % Calling a function with multiple outputs
   [sumRes, diffRes] = myOperations(8, 3);
   ```

4. **Anonymous Functions:**
   - Define anonymous functions for short, simple expressions.

   ```matlab
   % Anonymous function to square a number
   square = @(x) x^2;

   % Calling the anonymous function
   result = square(4);
   ```

5. **Built-in Functions:**
   - MATLAB has a wide range of built-in functions for various operations.

   ```matlab
   % Using built-in functions
   meanValue = mean([1, 2, 3, 4, 5]);
   ```

6. **Function Handles:**
   - Create function handles to pass functions as arguments or variables.

   ```matlab
   % Function handle example
   myFunction = @(x) x^2;
   result = myFunction(3);
   ```

These examples cover the basics of creating and using functions in MATLAB. Functions enhance code modularity, reusability, and readability. As you become more familiar with MATLAB, you can explore advanced topics like function handles, nested functions, and function input validation.
