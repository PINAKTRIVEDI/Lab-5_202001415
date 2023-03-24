# Lab-5_202001415
Analyzing the files from a selected repository.

I have selected the repository:- https://github.com/Mrinank-Bhowmick/python-beginner-projects/tree/main/projects/Alarm%20Clock

I am performing this analysis using "pylint".

Pylint is a tool that checks Python code for errors and warnings based on a set of predefined rules. The error and warning messages produced by pylint help to improve the quality and maintainability of the code.

The errors for "alarm_clock.py" file are as shown below:-

![image](https://user-images.githubusercontent.com/123732408/227476682-30272a66-f141-448d-9bfc-106d32287b88.png)

The errors for "clock.py" file are as shown below:-

![image](https://user-images.githubusercontent.com/123732408/227477390-5a96223d-7687-4891-8fba-1ba38485e0f9.png)

Running pylint on entire folder:-

![image](https://user-images.githubusercontent.com/123732408/227480883-d9ba3469-2ad0-4500-b07b-d43c6c2e2497.png)


Some of the errors are as shown below:-

=> Import Error

It occurs when the import statement of a module fails. It typically indicates that
the module you are trying to import cannot be found or there is an issue with the
module's code that is preventing it from being imported correctly.

=> Undefined variable

It occurs when you reference a variable that has not been defined in the current scope.

=> Redefined builtin

It is a warning error that is raised when you define a variable or function with the same name as a built-in Python function or keyword. This can lead to unexpected
behavior and bugs in your code.

=> Bad indentation

This warning is raised when there are inconsistent indentation levels in your
code. It could occur if you mix tabs and spaces, or if you use the wrong number
of spaces for indentation.

=> missing module

This warning is raised when a module is missing a docstring. A docstring is a
string literal that appears as the first statement in a module, function, class, or
method definition.

=> Invalid name

This warning is raised when a variable or function name does not conform to the
naming convention for Python code.

=> Trailing white space

This warning is raised when there is trailing whitespace at the end of a line.
(In pylint errors are define with error number : )

Error analysis using error codes:-

C0325: Unnecessary parens after '=' keyword (superfluous-parens)

This error message indicates that there are unnecessary parentheses after the assignment operator (=). To fix this, simply remove the parentheses around the assignment.

C0114: Missing module docstring (missing-module-docstring)

This warning message indicates that the module doesn't have a docstring. A docstring is a description of what the module does, and it is recommended to include it in all modules. To fix this, add a docstring to the module at the beginning of the file.

W0622: Redefining built-in 'enumerate' (redefined-builtin)

This warning message indicates that the built-in function 'enumerate' has been redefined. It is recommended to avoid redefining built-in functions to prevent unintended consequences. To fix this, choose a different name for the function.

W0401: Wildcard import tkinter (wildcard-import)

This warning message indicates that the module is importing all the names from the 'tkinter' module using a wildcard ('*'). This can make the code less clear and can cause naming conflicts. To fix this, import only the names that are needed from the 'tkinter' module explicitly.

W0401: Wildcard import threading (wildcard-import)

This warning message indicates that the module is importing all the names from the 'threading' module using a wildcard ('*'). This can make the code less clear and can cause naming conflicts. To fix this, import only the names that are needed from the 'threading' module explicitly.

C0116: Missing function or method docstring (missing-function-docstring)

This warning message indicates that a function or method doesn't have a docstring. A docstring is a description of what the function or method does, and it is recommended to include it in all functions and methods. To fix this, add a docstring to the function or method.

C0103: Function name "Threading" doesn't conform to snake_case naming style (invalid-name)

This error message indicates that the name of the function doesn't follow the snake_case naming style. Function names should be in lowercase letters with underscores separating words. To fix this, rename the function to follow the naming convention.

C0103: Variable name "t1" doesn't conform to snake_case naming style (invalid-name)

This error message indicates that the name of the variable doesn't follow the snake_case naming style. Variable names should be in lowercase letters with underscores separating words. To fix this, rename the variable to follow the naming convention.

C3001: Lambda expression assigned to a variable. Define a function using the "def" keyword instead. (unnecessary-lambda-assignment)

This error message indicates that a lambda expression is assigned to a variable. It is recommended to define a function using the 'def' keyword instead of using a lambda expression. To fix this, define a function using the 'def' keyword.

E1111: Assigning result of a function call, where the function has no return (assignment-from-no-return)

This error message indicates that the result of a function call is being assigned to a variable, but the function doesn't return anything. It is recommended to check if the function returns anything before assigning the result to a variable. To fix this, modify the code to 

Analysis of some of the errors:

1> error of new line

   calculator.py:93:0: C0304: Final newline missing (missing-final-newline)
   
-> This error removed by giving extra line.

2> Error of variable does not confirm

    calculator.py:12:4: C0103: Variable name "n2" doesn't conform to snake_case naming style (invalid-name)
    
    calculator.py:11:4: C0103: Variable name "n1" doesn't conform to snake_case naming style (invalid-name)
    
    calculator.py:26:4: C0103: Variable name "n1" doesn't conform to snake_case naming style (invalid-name)
    
    calculator.py:27:4: C0103: Variable name "n2" doesn't conform to snake_case naming style (invalid-name)
    
    calculator.py:37:0: C0103: Constant name "c" doesn't conform to UPPER_CASE naming style (invalid-name)
    
-> solve by moving the defination of my print to main() is one way to supress the message.


3> Missing docstring function error

   calculator.py:17:0: C0116: Missing function or method docstring (missing-function-docstring)
   
   calculator.py:25:0: C0116: Missing function or method docstring (missing-function-docstring)
   
   calculator.py:32:0: C0116: Missing function or method docstring (missing-function-docstring)
   
   calculator.py:5:0: C0116: Missing function or method docstring (missing-function-docstring)
   
   calculator.py:10:0: C0116: Missing function or method docstring (missing-function-docstring)
   
-> Implementing the function docstring in file

