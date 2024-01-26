# Global and Virtual environments

Now that we have installed Python, we mentioned that it comes with certain pre-installed basic libraries. But what happens when you want to use Python for a specific task and need to install additional packages? For this, Python has enabled `pip`, a recursive acronym for "Pip Installs Packages" or "Pip Installs Python", as its package manager to automate installation, update, and package removal.

However, installing new packages directly into the download of Python can have difficult consequences. This Python that we just installed is known as the **Global environment**. We mentioned that Python is an open-source interpreted programming language that goes through constant updates. For this reason, newer libraries developed on different versions of Python often go into conflict with libraries that have not gone through the same updates, and error messages start to pop up.

![badPythonEnv](https://github.com/mayraberrones94/CCI_technical/assets/35910638/807787ef-d5e2-4740-854b-f387b1602e90)
Dmitriy Zub, Dec 22, 2021. Python Virtual Environments tutorial using Virtualenv and Poetry. Place of publication: SerpApi. Available from: https://serpapi.com/blog/python-virtual-environments-using-virtualenv-and-poetry/#why_venv.

This image is a beautiful, chaotic example of what happens to your global environment when we do not have order in the different paths and versions of new packages.

To avoid this, a good practice when using Python is to use **virtual environments**. This environment allows for isolating package dependencies so they do not clash. For example, you may have two projects, one for computer vision and another for Natural Language Processing (NLP). Both of them use similar libraries but in different versions of Python. We can not install both versions system-wide, but we can create isolated environments for each project.



