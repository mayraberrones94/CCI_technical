# Global and Virtual environments

Now that we have installed Python, we mentioned that it comes with certain pre-installed basic libraries. But what happens when you want to use Python for a specific task and need to install additional packages? For this, Python has enabled `pip`, a recursive acronym for "Pip Installs Packages" or "Pip Installs Python", as its package manager to automate installation, update, and package removal.

However, installing new packages directly into the download of Python can have difficult consequences. This Python we just installed is the **Global environment**. We mentioned that Python is an open-source interpreted programming language that goes through constant updates. For this reason, newer libraries developed on different Python versions often conflict with libraries without the same updates, and error messages start to pop up.

![badPythonEnv](https://github.com/mayraberrones94/CCI_technical/assets/35910638/807787ef-d5e2-4740-854b-f387b1602e90)
Dmitriy Zub, Dec 22, 2021. Python Virtual Environments tutorial using Virtualenv and Poetry. Place of publication: SerpApi. Available from: https://serpapi.com/blog/python-virtual-environments-using-virtualenv-and-poetry/#why_venv.

This image is a beautiful, chaotic example of what happens to your global environment when we do not have order in the different paths and versions of new packages.

To avoid this, a good practice when using Python is to use **virtual environments**. This environment allows for isolating package dependencies so they do not clash. For example, you may have two projects, one for computer vision and another for Natural Language Processing (NLP). Both of them use similar libraries but in different versions of Python. We can not install both versions system-wide, but we can create isolated environments for each project.

**NOTE:** These environments are called containers because they do not interact with each other. However, this is only for the system. The folders are all available for all the environments. If you change a folder inside an environment, that change is permanent, so if you open it in another environment, it will have the previous changes. 

There are different ways to build Python environments:

**Very important** Please note that all of the steps mentioned on this page are recommended from original sources; try to follow them as faithfully as possible. If, in any step, something does not work as it should, contact a technician first before following any other instructions that need you to move things directly from your terminal. 

## Python environments (`venv`):

For this type of environment, the only requirement for your computer is to have a version of Python installed on it. `venv` is a Python module that supports lightweight virtual environments. 

**NOTE:** For this type of environment, you need to be familiar with how the terminal works, how you can move from one folder to another, and the Python versions you have installed. If you are unfamiliar with these requirements, please refer to the How to use Anaconda section.

From Python 3.3 onwards, `venv` should be included in the commands available. To create a virtual environment with this, please open your terminal:

**NOTE:** If you have not yet installed Python on your computer, please refer to the Installing Python section of the wiki.

**macOS**

To enter the terminal, you can search it directly from the Launchpad or application folder. Type `Command` + `Space bar` and type terminal for a shortcut. First, we must ensure you are in the folder where you want to save the environment. When you open the terminal, you should see only your user name:

<img width="580" alt="Python_terminal" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/a6cde0f7-1573-488c-8533-aaa591dcbc96">

For this example, I am going to access my Documents folder. You can access whatever folder you wish to save your environment on. 

**Why is this important?** If you save a virtual environment with the same name in the same folder, the terminal will interpret it as you want to rewrite it, and you will lose the information from the previous one. Before creating new environments, make sure that the name and folder you choose differ from previous ones. 


```python
python -m venv [name of the environment]
```

Inside of the brackets, you can change it to whatever name you want. Just make sure that the name of the environment is something easy to remember, or write it down somewhere. The name should also follow the terminal rules: if you are going to name something with more than one word, you need to hyphenate the words with an underscore (_). Example: `python -m venv example_environment`.

The way you activate it is while inside the folder where you created the environment, call `source [name of the environment]/bin/activate`. The name in front of the dollar sign should change to the name of the environment you are currently in. 

Example:

<img width="674" alt="Captura de Pantalla 2024-02-13 a la(s) 9 29 28 a m" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/0f2a604a-8543-4a6b-b4fc-7d99161d9b29">


**Windows**

For the Windows OS you also need to have previously installed Python.

**IMPORTANT** If you installed Python by downloading the installer directly from the Python page, you might need to add the path to the environment variables of your computer. Please see the section on how to do that in the "Add path to environment" section. If you are not familiar with the path and what it means to add it to the environment variables, please continue with the next steps.


If you have Python already in your Path variables, you can just use the same arguments as the macOS instructions. ( Example: `python -m venv example_environment`) Please note that the same rules apply to Windows, so make sure to name the environment something unique and easy to remember, and also select the correct folder for your environment.

## Conda environments

Another way to create environments in Python is to use the Anaconda distribution. For this, we have two options: we can download Anaconda from the official distribution or a more light version of Anaconda called Miniconda. 

**Which version do I need?** These two versions are from the same distribution and are widely used for data science and scientific computing. The main difference between the two is the size of the installation. Anaconda requires at least 3 GB of free disk space, while Miniconda only requires 400 MB (Something you need to take into consideration if you do not have enough space available on your computer). Anaconda comes with a large array of pre-installed packages and a very user-friendly graphical interface that can favor those who are not very familiar with the use of the terminal or command line prompts. Miniconda only includes the `conda` function and Python in its installation.

If you go for the Anaconda version:

**macOS**

If you go to the official Anaconda page (https://www.anaconda.com/download#downloads), you will see the Download button for your OS. If you are using macOS, it is also important to know if your hardware settings are an Intel chip or an M1/M2/M3 chip. 

<img width="1063" alt="Screenshot 2024-02-12 at 11 00 56" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/403c2bfd-05f0-4c26-abb5-14ee2977cd7d">

You can check this by going to the Apple at the top left corner of your screen and clicking on About this Mac. 

<img width="367" alt="Screenshot 2024-02-12 at 11 04 31" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/b333860f-c459-4e52-80a2-3619dc8d4619">


This should prompt a Window that will say the chip your computer has:

<img width="295" alt="Screenshot 2024-02-12 at 11 04 45" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/e7201e37-d2a4-4a95-ae64-37902a741409">

Go back to the Downloads page on Anaconda and choose the right setting for your computer. 

**NOTE:** You can also click on `More info` to see all the different settings on your computer. 

<img width="718" alt="Screenshot 2024-02-12 at 11 05 01" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/6d98dff9-91f8-49c2-ae6a-7fab01a50f5f">

Once the package is done loading, you can choose the predetermined installation and click install. If your terminal was opened, please relaunch it, you will now be able to see the pre fix in your user name as `(base)`. Which means that you are in the base or root environment. We explain this later on.

It goes from:

<img width="403" alt="Screenshot 2024-02-12 at 11 16 26" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/cea1fe81-dda3-4c76-8025-aa09ea334856">

To look something like this:

<img width="449" alt="Captura de Pantalla 2024-02-13 a la(s) 10 02 38 a m" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/a11a51b0-0d4b-4028-82c0-7bb44f3d9a59">

## For Windows users:

For Windows, there is only one universal installer, so it does not matter the version of Windows that you are using. It is only important to know that it is only available for the 64-bit version. If your computer is a 32-bit, please look into the Anaconda archive (https://docs.anaconda.com/free/anaconda/install/old-os/).

<img width="1048" alt="image" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/4495fa11-f067-4259-beed-dafcb5cf96e4">

Follow the installation process. Same as with the Python installation, this installer is going to ask you if you want to add this software to your path variables. If you are not sure or do not understand fully what path does, do not activate this function. We can change it later on if you need it.

**NOTE** If you do not want to add Conda to your path variables, you can use the command prompt directly from the Anaconda Navigator. Otherwise, all the other Windows terminals will not have the `conda` prompt.

<img width="277" alt="image" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/b0051618-1bae-430c-84e6-667f521fe977">


<img width="1179" alt="image" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/deb99628-bdf9-4f59-9a0c-1eed193f2ca1">


# Installing Miniconda

**Note:** Please be mindful that Miniconda has no user interface and only offers the `conda` prompt and Python. It also requires general knowledge of how the terminal works. 

## Graphical installer:

**macOS**

You must download the Miniconda installer from the official page (https://docs.anaconda.com/free/miniconda/). From here, you can choose the Intel or the M1/2/3 chip version and the bash or pkg versions. We strongly recommend using the bash version since the pkg may skip the "Destination select" process, failing the installation.

**bash** 
- Once you download the document, locate where it is stored (it is most likely in the Downloads folder).
- Go to a new terminal in your computer (`Command` + `Space bar` type terminal + `Enter`)
- Go into the folder where you have the bash file stored (Ej. `cd Downloads`); you can verify it is there by running `ls`.
- This is an optional step, but we recommend verifying the download to ensure everything will run correctly. In your terminal run `shasum -a 256 filename` replacing `filename` with the downloaded file name. If it does not raise any error, follow the next step.
- Run  `bash <conda-installer-name>-latest-MacOSX-x86_64.sh`. Replace the `<conda-installer-name>` with the downloaded file's name.
- Once the process is finished, please close and reopen your terminal (`Command` + `q` to close/reboot the program completely. You can see if this was successful by clicking `Command` + `tab`. It should show you all the applications you have opened. Make sure that the terminal does not show there).
- To verify the installation, open a terminal window and run `conda list`. If you installed everything correctly, a list of all the installed packages should appear.

**Windows**


  




