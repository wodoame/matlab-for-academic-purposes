Sure! Array indexing in MATLAB allows you to access and manipulate individual elements or subsets of elements within an array or matrix. Here are some common indexing techniques:

### 1. **Single Element Indexing:**
   - Access a single element using its row and column indices:
     ```matlab
     A = [1, 2, 3; 4, 5, 6; 7, 8, 9];

     % Access the element in the second row and third column
     element = A(2, 3);
     ```

### 2. **Row or Column Indexing:**
   - Access an entire row or column using a single index:
     ```matlab
     A = [1, 2, 3; 4, 5, 6; 7, 8, 9];

     % Access the second row
     row = A(2, :);

     % Access the third column
     column = A(:, 3);
     ```

### 3. **Submatrix Indexing:**
   - Access a submatrix by specifying ranges for rows and columns:
     ```matlab
     A = [1, 2, 3; 4, 5, 6; 7, 8, 9];

     % Access a submatrix (rows 1 to 2, columns 2 to 3)
     submatrix = A(1:2, 2:3);
     ```

### 4. **Linear Indexing:**
   - Access elements using a single index that linearly traverses the matrix column-wise:
     ```matlab
     A = [1, 2, 3; 4, 5, 6; 7, 8, 9];

     % Access the element in the fifth position
     element = A(5);
     ```

### 5. **Logical Indexing:**
   - Use logical arrays to index elements based on a specified condition:
     ```matlab
     A = [1, 2, 3; 4, 5, 6; 7, 8, 9];

     % Logical indexing to get elements greater than 5
     elements_gt_5 = A(A > 5);
     ```

### 6. **Assigning Values to Elements:**
   - You can assign new values to specific elements or submatrices:
     ```matlab
     A = [1, 2, 3; 4, 5, 6; 7, 8, 9];

     % Change the value of the element in the second row and third column
     A(2, 3) = 10;
     ```

### 7. **Using `end` Keyword:**
   - The `end` keyword is used to refer to the last index along a particular dimension:
     ```matlab
     A = [1, 2, 3; 4, 5, 6; 7, 8, 9];

     % Access the last element in the second row
     last_element = A(2, end);
     ```

These examples cover basic array indexing techniques in MATLAB. MATLAB's flexible indexing capabilities make it easy to manipulate and extract information from arrays and matrices. Experiment with these methods to get a hands-on understanding.

### NOTE
  - If you try to refer to elements outside an array on the right side of an assignment statement, MATLAB throws an error.
    ```matlab
      test = A(4,5)
    ```
  - However, on the left side of an assignment statement, you can specify elements outside the current dimensions. The size of the array increases to accommodate the newcomers.
    ```matlab
      A(4,5) = 17

     1     2     3     4     0
     5     6     7     8     0
     9    10    11    12     0
    13    14    15    16    17
    
    ```
