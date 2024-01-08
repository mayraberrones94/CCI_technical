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

name = 'My name is Mayra' #String variable
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
My name is Mayra
Item 1

Student 4:
Age: 23
Gender: non-binary
Major: Engineering
```

For simple variables like 'name', we can just call the variable's name. For the list and dictionaries, we need to have an awareness of the amount of objects that it has, so we can call them by their index. This is easy when we can keep track of the amount of things inside these types of containers. For the cases when we have more objects inside containers, Python has libraries that make navigating and using the data inside those structures easier. 

** IMPORTANT NOTES: **

The most common mistakes when dealing with declaring variables can be avoided with certain good practices.

- When declaring variables, remember that Python has certain rules. For example, Python is lower/higer case sensitive. So if you declare a variable as `name` and then call it later as `Name` it is going to raise an error of a variable that has not been declared yet.
- 
