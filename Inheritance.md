# Functions, classes and libraries

In the previous page about basic data types, we discussed one of Python's capabilities as an object-oriented programming language, and an important aspect of that is the support for classes and multiple inheritances. This can be done by libraries or code grouped into modules, classes and packages. 

We mentioned using keywords by Python and how those keywords have assigned capabilities. Some of these keywords are there in place to facilitate a process or a task. In the case of functions, classes and packages, we can build our programming tasks. Functions are the programming structure we use when we have a repetitive task inside of our program, and by using functions, it is like we are just using a template of a task and filling it out with the objects that we need when we need them, and then free that slot of memory when it is no longer necessary. This structure is excellent not only for maintaining a clean and tidy code but also helps to avoid memory problems later on.

So let's see an example of a function:

```python
def sum_of_numbers (number_1, number_2):
  result = number_1 + number_2
return result

print(sum_of_numbers(90, 1))
```

In the last code, the function `sum_of_numbers` takes two integers or float numbers and sums them; the output, in this case, is 91. But in this function, we assume that the user is always going to input a number and not, for example 


```python
def sum_of_numbers (number_1, number_2):
  try:
    result = number_1 + number_2
  except:
    result = 'This function requieres numbers'
  return result

print(sum_of_numbers(90, 1))
```

```python
print(result)
```
