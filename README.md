# Lab-5_202001415
Analyzing the files from a selected repository.

I have selected the repository:- https://github.com/Mrinank-Bhowmick/python-beginner-projects/tree/main/projects/Alarm%20Clock


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

C0304 : Missing final newline

This warning is raised when there is no final newline at the end of a file. This can
cause issues with some text editors and tools.

C0116 : Missing function docstring

Missing function or method docstring used when a function or method has no
docstring. Some special methods like __init__, protected, private functions,
setters and deleters do not require a docstring (learn more from testscases).

C0415 : Import outside top level

Used when an import statement is used anywhere other than the module

toplevel.Move this import to the top of the file  

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

