NOTE: Please complete the whole reading before installing anything, as some parts highlight older practices and do not reflect the current way to install Python.

If you are brand new to the Python programming language, you first need to have it properly installed on your computer. To run a Python program, you will need a Python interpreter. If you try to install Python from the official page python.org, you are essentially just downloading an executable program that operates a Python interpreter and holds a large suite of useful tools and functions that you can utilize in your code. This is known as the Python standard library. 

<img width="1221" alt="Python_dowload" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/3bf78149-4f7f-4003-8e1e-5304f5a43d47">

For the example image, the page usually picks up on the operating system of the computer you are using. If you are looking for a different format or a specific release version, you can manually search for it in the Active Python releases.

# What are Python releases?

Python is community-based and open-sourced, meaning it is free to use, and anyone can participate in improving, maintaining and releasing their own libraries. This adds great functionality to the language but also requires the periodic release of newer versions, which helps to add these newer features and fixes previous bugs. All Python versions are formatted as `A.B.C`; the first number is a major release, the second one a minor release, and the third represents patches to fix bugs. For example, as of writing this, the current release of Python is **3.12.1**. 

## So, which Python version do I need?

It is best to check the Python version that has fewer issues with the libraries and packages that you know you are going to need. For this, we will work with environments, which are little containers that will help you keep your libraries and Python versions running as smoothly as possible. But first, let's help you install Python on your computer.

# For Windows:

If you are new to Python and looking to get started quickly, you can install it by going directly to the Microsoft Store page

Once you download the `.exe` file of the latest Python version (right now, it is not important to look for different versions), follow the installation guide. Remember to select either the Windows x86-64 executable installer for 64-bit or the Windows x86 executable installer for 32-bit, depending on your own computer specifications. You can see which one you have by following the next steps:

1. Click the start button at the bottom left corner.
2. Select or search for "Settings"

![Windows_screen](https://github.com/mayraberrones94/CCI_technical/assets/35910638/841c2627-4cc9-4752-868b-6e0434b10599)

3. In "Settings", select the "System" tab.

![systems_page](https://github.com/mayraberrones94/CCI_technical/assets/35910638/7f806b9b-41eb-4418-ba89-5023705b162d)

4. Scroll all the way down on the left panel and click "About". The information you need is under "Device specifications" in the System type. 

![System_about](https://github.com/mayraberrones94/CCI_technical/assets/35910638/6c24e493-78c0-492e-9552-a10db789aa89)

**IMPORTANT:** Please note that drivers made for the 32-bit version of Windows will not work correctly on a computer running on a 64-bit version and vice versa.

Now that we have the correct installer for your computer run the file. A dialogue window will appear, and there are some different things we can do with it.


![Python_setup](https://github.com/mayraberrones94/CCI_technical/assets/35910638/cd3029c1-be3f-4e1c-86e7-eab8f01a0e51)

- The default path for installation is in the directory of the current Windows user. The Install launcher for all users (recommended) checkbox is checked default. This means every user on the machine will have access to the py.exe launcher. You can uncheck this box to restrict Python to the current Windows user.

- There is another checkbox that is unchecked by default called Add Python to PATH. There are several reasons why you might not want Python on PATH, so make sure you understand what this does before clicking on it.

**IMPORTANT:** If you do not know what PATH is, we strongly recommend you use the Microsoft Store Package instead of this installer. The Microsoft package is directed to people who are new to Python and focused primarily on learning the language rather than building professional software.


Installing it lets you go to your terminal and execute a Python script. Assuming that you know how to deploy and work with the terminal (command tool) in your computer, once you have an interpreter installed, you can run a Python code by going to the folder where the py file is stored (from the terminal), and run:

```
python my_script.py
```

Being 'my_script' the name of our dummy code. This will instruct the Python interpreter stored on your computer to read that file. Assuming that the code obeys the grammatical rules of Python and the instructions in the code have to provide an output, this will appear in the terminal window. Again, this is an example of a very simple code. Some codes also require input from the user, and for that, we will need further tools.


## 

