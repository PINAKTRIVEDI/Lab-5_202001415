# Lab-5_202001415
Analyzing the files from a selected repository.

I have selected the repository:- https://github.com/Mrinank-Bhowmick/python-beginner-projects/tree/main/projects/Alarm%20Clock


The errors for "alarm_clock.py" file are as shown below:-

![image](https://user-images.githubusercontent.com/123732408/227476682-30272a66-f141-448d-9bfc-106d32287b88.png)

Content:-

Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Try the new cross-platform PowerShell https://aka.ms/pscore6

PS C:\Users\student\Downloads\python-beginner-projects-main\projects\Alarm Clock> python -m pylint alarm_clock.py
************* Module alarm_clock
alarm_clock.py:39:0: C0325: Unnecessary parens after '=' keyword (superfluous-parens)
alarm_clock.py:1:0: C0114: Missing module docstring (missing-module-docstring)
alarm_clock.py:5:0: W0622: Redefining built-in 'enumerate' (redefined-builtin)
alarm_clock.py:1:0: W0401: Wildcard import tkinter (wildcard-import)
alarm_clock.py:5:0: W0401: Wildcard import threading (wildcard-import)
alarm_clock.py:12:0: C0116: Missing function or method docstring (missing-function-docstring)
alarm_clock.py:12:0: C0103: Function name "Threading" doesn't conform to snake_case naming style (invalid-name)
alarm_clock.py:13:4: C0103: Variable name "t1" doesn't conform to snake_case naming style (invalid-name)
alarm_clock.py:17:0: C0116: Missing function or method docstring (missing-function-docstring)
alarm_clock.py:217:13: C3001: Lambda expression assigned to a variable. Define a function using the "def" keyword instead. (unnecessary-lambda-assignment)
alarm_clock.py:218:0: E1111: Assigning result of a function call, where the function has no return (assignment-from-no-return)
alarm_clock.py:218:0: C0103: Constant name "button" doesn't conform to UPPER_CASE naming style (invalid-name)
alarm_clock.py:1:0: W0614: Unused import(s) enum, sys, types, TclError, re, wantobjects, TkVersion, TclVersion, READABLE, WRITABLE, EXCEPTION, EventType, Event, NoDefaultRoot, Variable, IntVar, DoubleVar, BooleanVar, mainloop, getint, getdouble, getboolean, Misc, CallWrapper, XView, YView, Wm, Tcl, Pack, Place, Grid, BaseWidget, Widget, Toplevel, Canvas, Checkbutton, Entry, Listbox, Menu, Menubutton, Message, Radiobutton, Scale, Scrollbar, Text, Image, PhotoImage, BitmapImage, image_names, image_types, Spinbox, LabelFrame, PanedWindow, NO, FALSE, OFF, YES, TRUE, ON, N, S, W, E, NW, SW, NE, SE, NS, EW, NSEW, CENTER, NONE, X, Y, BOTH, TOP, RIGHT, BOTTOM, RAISED, SUNKEN, FLAT, RIDGE, GROOVE, SOLID, HORIZONTAL, VERTICAL, NUMERIC, CHAR, WORD, BASELINE, INSIDE, OUTSIDE, SEL, SEL_FIRST, SEL_LAST, END, INSERT, CURRENT, ANCHOR, ALL, NORMAL, DISABLED, ACTIVE, HIDDEN, CASCADE, CHECKBUTTON, COMMAND, RADIOBUTTON, SEPARATOR, SINGLE, BROWSE, MULTIPLE, EXTENDED, DOTBOX, UNDERLINE, PIESLICE, CHORD, ARC, FIRST, LAST, BUTT, PROJECTING, ROUND, BEVEL, MITER, MOVETO, SCROLL, UNITS and PAGES from wildcard import of tkinter (unused-wildcard-import)
alarm_clock.py:5:0: W0614: Unused import(s) functools, get_ident, get_native_id, ThreadError, TIMEOUT_MAX, setprofile, getprofile, settrace, gettrace, Lock, RLock, Condition, Semaphore, BoundedSemaphore, Barrier, BrokenBarrierError, ExceptHookArgs, excepthook, Timer, current_thread, currentThread, active_count, activeCount, enumerate, main_thread, WeakSet, namedtuple, stack_size, local and lock from wildcard import of threading (unused-wildcard-import)

------------------------------------------------------------------
Your code has been rated at 5.71/10 (previous run: 5.71/10, +0.00)


The errors for "clock.py" file are as shown below:-

![image](https://user-images.githubusercontent.com/123732408/227477390-5a96223d-7687-4891-8fba-1ba38485e0f9.png)

CONTENT:-
************* Module clock
clock.py:1:0: C0114: Missing module docstring (missing-module-docstring)
clock.py:9:0: C0116: Missing function or method docstring (missing-function-docstring)

-----------------------------------
Your code has been rated at 8.46/10

Running pylint on entire folder:-

************* Module ALARM
ALARM:1:0: F0001: No module named ALARM (fatal)
************* Module CLOCK
CLOCK.py:1:0: C0114: Missing module docstring (missing-module-docstring)
CLOCK.py:1:0: C0103: Module name "CLOCK" doesn't conform to snake_case naming style (invalid-name)
CLOCK.py:9:0: C0116: Missing function or method docstring (missing-function-docstring)

------------------------------------------------------------------
Your code has been rated at 0.00/10 (previous run: 8.46/10, -8.46)

Some of the errors are as shown below:-

=> Import Error
It occurs when the import statement of a module fails. It typically indicates that
the module you are trying to import cannot be found or there is an issue with the
module's code that is preventing it from being imported correctly.
=> Undefined variable
It occurs when you reference a variable that has not been defined in the current
scope.
=> Redefined builtin
It is a warning error that is raised when you define a variable or function with the
same name as a built-in Python function or keyword. This can lead to unexpected
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

