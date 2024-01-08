# Python 

Python is a powerful object-oriented programming language (OOP). It is important to understand the basic concept of OOP to navigate Python with more ease. 

In simple terms, in OOP an object serves as a container. They can contain data, attributes or properties, and methods. Objects are made to interact with one another, in a way that serves the structure for the program we want to execute. When used correctly, this makes programing easier to modify, debug and maintain. Different languages have different ways to declare an object. 

Python is one of the most popular OOP programing languages for Data Science, mostly because it holds a vast number of standard libraries that support many common tasks like searching text with regular expressions, reading and modifying files, etc.

## Basic data types

As we mentioned before, different programming languages have different ways to declare an object. Python for example has a variety of basic data types that it recognizes when you assign them to a variable. For example:

```python
# How do we assign value to the variables?

number_1 = 9 #Integer number
number_2 = 9.8 #Float number

name = 'My name is J. Doe' #String variable
grocery_list = ['Item 1', 'Item 2', 23, '2345'] #This is a list of mixed items

#The next one is going to be a dictionary structure
students = {
    'student1': {'age': 20, 'gender': 'male', 'major': 'Computer Science'},
    'student2': {'age': 22, 'gender': 'female', 'major': 'Biology'},
    'student3': {'age': 21, 'gender': 'male', 'major': 'Psychology'},
    'student4': {'age': 23, 'gender': 'non-binary', 'major': 'Engineering'},
    'student5': {'age': 19, 'gender': 'female', 'major': 'Mathematics'}
}

```

For each one, we do not have to tell Python what type of variable it is. If it’s a number and it does not have a decimal point, it is going to assume that it is an integer; otherwise, it is a float number. If it has a simple or double comma (‘ or “), it is assumed to be a string. 

For the list or the dictionary, there are different types of containers. In those cases, they have several different variables declared inside of them, so they can be referred to as a container of containers, and they have to be addressed differently than a simple variable. For example:

```python

print(name)
print(grocery_list[0])

print("Student 4:")
print("Age:", students['student4']['age'])
print("Gender:", students['student4']['gender'])
print("Major:", students['student4']['major'])
```

The output of the last code will be:

```
My name is J. Doe
Item 1

Student 4:
Age: 23
Gender: non-binary
Major: Engineering
```

For simple variables like 'name', we can just call the variable's name. For the list and dictionaries, we need to be aware of the number of objects that it has, so we can call them by their index. This is easy when we can keep track of the amount of things inside these types of containers. For the cases when we have more objects inside containers, Python has libraries that make navigating and using the data inside those structures easier. 

**IMPORTANT NOTES:**

The most common mistakes when declaring variables can be avoided with certain good practices.

- When declaring variables, remember that Python has certain rules. For example, Python is lower/higher case sensitive. So if you declare a variable as `name` and then call it later as `Name` it is going to raise an error of a variable that has not been declared yet.
- Be aware of the names of your variables. Python has a way of assigning memory to the variables you declare, where if you name another variable the same way, it will update the information with the new data. So, when you call the variable again and receive unexpected results, the cause might be that you reused the name of an old variable.
- Lastly, for this section, another common mistake is trying to name a variable, a keyword of Python. As we mentioned at the beginning, Python has many built-in keywords that make it easier to navigate basic programming functions. If you go back and see the example code, you can see that we did not have to declare the variable `print`, and that is because it is one of the Python keywords that has the action of printing the object selected. Because these keywords already contain something (in this case, a function) they can not be called to name any other object. Usually, programming editors will have a different color for these keywords, but in case you are curious, [here](https://realpython.com/python-keywords/) you can see a list of all the keywords Python has built-in. On the next page, we will discuss keywords assigned to libraries or classes.


(Another way of seeing them is to type in the following code:)

```python
help("keywords")
```

```
Here is a list of the Python keywords.  Enter any keyword to get more help.

False               class               from                or
None                continue            global              pass
True                def                 if                  raise
and                 del                 import              return
as                  elif                in                  try
assert              else                is                  while
async               except              lambda              with
await               finally             nonlocal            yield
break               for                 not
```

- 
