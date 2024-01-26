# 1. Getting started - Installing Python (Mac OS)

For Mac users, there are different ways to install Python: by going to the official Python page and installing it directly from the page or using the Anaconda package (which we will show in another post).

**Important** The Homebrew package manager is another popular method for installing Python on macOS. However, the Python distribution offered by Homebrew isn’t controlled by the Python Software Foundation and could change at any time. The most reliable method on macOS is to use the official installer, especially if you plan on programming Python GUI with Tkinter (Homebrew doesn’t include the Tcl/Tk dependency required by the Tkinter module).

**Note:** Mac OS no longer has a pre-installed version of Python in their systems (Starting from macOS Catalina).

## Downloading the installer:

Most recent versions of Mac computers no longer have a pre-installed version of Python, and if your computer is brand new, most likely, it does not have it installed. Either way, it is always good practice to check if we have a previous version of Python installed so the packages do not clash.

To see if you have installed any Python version, launch the terminal of your computer by:

1. Searching for it in the Applications folder.
2. `Command` + `Space bar` and typing "Terminal"

and type `python --version` in it and hit `Enter`. If it’s not installed, you will see `command not found: python`. If installed, it will show you which version you have installed. Alternatively, you can type `Python`, and the terminal will automatically enter a Python running script, showing the Python version you have and the date of its release.

<img width="578" alt="Python_mac" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/ff02ad0f-6b32-471e-b294-10c8b3043992">

If Python is not installed, you can then use the installer. When you open the official page with your Mac, it automatically gives you the option for the latest version of the MacOS operating system. 

<img width="1220" alt="Python_installerMac" src="https://github.com/mayraberrones94/CCI_technical/assets/35910638/30694d49-2b56-4f10-adc7-28bcae857d30">

Run the installer and follow the instructions. When you reach the installation type section, ensure enough space in your disk to install this package. 

![Installation_type](https://github.com/mayraberrones94/CCI_technical/assets/35910638/e3ffb33c-2c34-4f58-8d4f-3650d7337c6f)

If you have partitions in your disk and want to change the installation location, you can select this by clicking the `Change Install Location` and choosing the disk you want. If not, click  `Install`. The installation might take 5 to 10 minutes, depending on your internet connectivity. When the installer is finished copying files, double-click the `Install Certificates` command in the finder window to ensure your SSL root certificates are updated.

Restart your terminal (you can close it and open it in a new window) and repeat the process of checking the Python version. It should show you the version you have just installed.

