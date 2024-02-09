# Global and Virtual environments

Now that we have installed Python, we mentioned that it comes with certain pre-installed basic libraries. But what happens when you want to use Python for a specific task and need to install additional packages? For this, Python has enabled `pip`, a recursive acronym for "Pip Installs Packages" or "Pip Installs Python", as its package manager to automate installation, update, and package removal.

However, installing new packages directly into the download of Python can have difficult consequences. This Python that we just installed is known as the **Global environment**. We mentioned that Python is an open-source interpreted programming language that goes through constant updates. For this reason, newer libraries developed on different versions of Python often go into conflict with libraries that have not gone through the same updates, and error messages start to pop up.

![badPythonEnv](https://github.com/mayraberrones94/CCI_technical/assets/35910638/807787ef-d5e2-4740-854b-f387b1602e90)
Dmitriy Zub, Dec 22, 2021. Python Virtual Environments tutorial using Virtualenv and Poetry. Place of publication: SerpApi. Available from: https://serpapi.com/blog/python-virtual-environments-using-virtualenv-and-poetry/#why_venv.

This image is a beautiful, chaotic example of what happens to your global environment when we do not have order in the different paths and versions of new packages.

To avoid this, a good practice when using Python is to use **virtual environments**. This environment allows for isolating package dependencies so they do not clash. For example, you may have two projects, one for computer vision and another for Natural Language Processing (NLP). Both of them use similar libraries but in different versions of Python. We can not install both versions system-wide, but we can create isolated environments for each project.

**NOTE:** These environments are called containers because they do not interact with each other. However, this is only for the system. The folders are all available for all the environments. If you change a folder inside an environment, that change is permanent, so if you open it in another environment, it will have the previous changes. 

There are different ways to build Python environments:

## Python environments (`venv`):

For this type of environment, the only requirement for your computer is to have a version of Python installed on your computer. `venv`is a Python module that supports lightweight virtual environments. 

**NOTE:** For this type of environment, you need to be familiar with how the terminal works, how you can move from one folder to another, and the Python versions you have installed. If you are unfamiliar with these requirements, please refer to the How to use Anaconda section.

From Python 3.3 onwards, `venv` should be included in the commands available. To create a virtual environment with this, please open your terminal:

**NOTE:** If you have not yet installed Python on your computer, please refer to the Installing Python section of the wiki.

**macOS**

To enter the terminal, you can search it directly from the Launchpad or application folder. For a shortcut, type `Command` + `Space bar` and type terminal. First, we need to ensure that you are in the folder where you want to save the environment. When you open the terminal, you should see only your user name:

<img width="580" alt="Python_terminal" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/a6cde0f7-1573-488c-8533-aaa591dcbc96">

For this example, I am going to access my Documents folder. You can access whatever folder you wish to save your environment on. 

**Why is this important?** If you save a virtual environment with the same name in the same folder, the terminal is going to interpret it as you want to rewrite the environment, and you will lose the information from the previous one. Before you create new environments, make sure that the name and folder you choose are different than previous ones. 


```python
python -m venv [name of the environment]
```

Inside of the brackets, you can change it to whatever name you want. Just make sure that the name of the environment is something easy to remember, or write it down somewhere. The name should also follow the rules of the terminal: if you are going to name it something with more than one word, you need to hyphenate the words with an underscore (_). Example: `python -m venv example_environment`.

The way you activate it is, while being inside the folder where you created the environment, call `source [name of the environment]/bin/activate`. The name in front of the dollar sign should change to the name of the environment you are currently on. 

**Windows**

For the Windows OS you also need to have previously installed Python.

**IMPORTANT** If you installed Python by downloading the installer directly from the Python page, you might need to add the path to the 




