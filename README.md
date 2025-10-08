# ELEC2645 Unit 1.2 Activity 2 - 2D Arrays

Arrays can be 2 dimensions or higher and follow a similar syntax as for a 1D array: 

```c
char array[2][3] = { {'a','b','c'}, {'d','e','f'}};
```
where the elements for each row are contained in their own `{}`. 

We can find out the size of a variable by using `sizeof`, which returns how many *bytes* the variable takes in memory. 

- `sizeof(array)` - returns the size of the *whole* array in bytes
- `sizeof(array[0])` - for a 1D array returns the size of the element or for a 2D array returns the size of a row
- `sizeof(array[0][0])` - for a 2D array returns the size of a single element

We can use the function like so `int b = sizeof(a)`. Technically the output is in a special type `size_t` but we can use `int` for our purposes for now.


### 1 Run code
The program `main.c` needs compiling before it can run. In the terminal you can type `gcc main.c -o main.out` and then `./main.out` to run the new program.

### 2 The assignment
The program initialises a 2D array, but the calculations are not finised. Complete the steps in the code to print
- Total size
- The number of rows and columns
- The value of the element in the second row and third column
- The sum of all elements
- The average of all elements

### 3 Test command
In the terminal run `make test` which will build `main.c` to create `main.out` (if not done already) and then it will run the test script `test.sh`. These instructions are defined in the `Makefile`. If your code is correct you should see `-d[o_0]b All tests passed :D`

### 4 Submit Solution
Once you have solved the task, you must submit the changes so the autograder runs. To do this you must commit changes and then publish them to the repository. 

To do this:
- Switch to `Source Control` tab on the left hand side
- Stage the files you have changed by clicking `+` by each file, this is normally just the `.c` code files you have changed. Or stage all files by `+` at the top of the list
- Type a _meaningful_ commit message in the text box then hit `Commit`
- Hit `Sync Changes` to send updates to to the remote repository on GitHub. If the green button does not change to `Sync Changes` you can still submit hitting the `...` just above the message box and selecting `Push`
- The autograder will run in the background, you can check the results on the repository page. 
- You can find the link to the repository page either from the original GitHub classroom invite link, or by switching back to the `Explorer` tab, right click in the blank space under all of the files and then selecting `share` then `Copy github.dev Link`  