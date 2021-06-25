# Session 7
Session 7 - Functional Parameters

### Description of the module:
This is for session 7 assignment on the various scopes and closures concepts in Python. It includes usage of concepts like global scope, local scope, nonlocal scope, closure and free variable etc.  

### Problem Statement

1. Write a closure that takes a function and then check whether the function passed has a docstring with more than 50 characters. 50 is stored as a free variable (+ 4 tests) - 200  
2. Write a closure that gives you the next Fibonacci number (+ 2 tests) - 100  
3. We wrote a closure that counts how many times a function was called. Write a new one that can keep a track of how many times add/mul/div functions were called, and update a global dictionary variable with the counts (+ 6 tests) - 250  
4. Modify above such that now we can pass in different dictionary variables to update different dictionaries (+ 6 tests) - 250  
5. Once done, upload the code to github, run actions, and then proceed to answer S7 - Assignment Solutions.  

### Implementation
##### Function for Ques. 1
**docstring_checker:** This function creates a closure with a free variable check_length = 50. The function doesn’t need any input. The function returns the inner function which evaluates whether the passed function has a valid docstring length.  

**docstring_checker_inner:** This function checks for validity of docstring by checking it's length Currently the docstring length > 50 is assumed to be valid. The function takes a function name as input. The function returns True or False depending on whether the passed function has a valid docstring length.  

##### Function for Ques. 2
**next_fibonacci_number:** This function creates a closure for identifying next Fibonacci number. The function doesn’t need any input. The function returns you the inner function which gives the next Fibonacci number every time the function is run.  

**next_fibonacci_number_inner:** This function returns the next fibonacci number in the series. Currently the docstring length > 50 is assumed to be valid. The function takes an integer n as input. The function returns the next fibonacci number in the series.  



##### Function for Ques. 3
**add:** A custom function to add two given numbers.  

**mul:** A custom function to multiply two given numbers.  

**div:** A custom function to divide two given numbers. It also checks that the denominator is not zero.  

**func_call_counter:** This function creates a closure that can keep count of how many times a function was called. The function takes function name as input. The function returns you the inner function which returns a dictionary with fuction names and their total runs so far as a key value pair.  

**func_call_counter_inner:** This function returns a dictionary with fuction names and their total runs so far as a key value pair. The function any number of arguments as inputs. The function returns a dictionary with fuction names and their total runs so far as a key value pair.  

##### Function for Ques. 4
**func_call_counter_user:** This function creates a closure that can keep count of how many times a function was called. The function takes a dictionary as input. The function returns you the inner function which returns the updated dictionary with fuction names and their total runs so far as a key value pair.  

**func_call_counter_user_inner:** This function returns an inner function. The function takes function name as input. The function returns an inner function which in turn returns a dictionary with fuction names and their total runs so far as a key value pair.  

**func_call_counter_user_innermost:** This function returns a dictionary with fuction names and their total runs so far as a key value pair. The function any number of arguments as inputs. The function returns a dictionary with fuction names and their total runs so far as a key value pair.  


### Test Cases:

Some basic test cases are written to test README (number of words, keywords covered, proper headings for README), naming standards and indentations. A few function wise test cases have also been added