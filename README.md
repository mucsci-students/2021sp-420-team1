# CSCI 420 (Spring 2021) MontyPython UML Editor

This command line program creates a text representation of a UML diagram though user input. The program’s capabilities include adding, deleting, displaying, and modifying UML diagram elements. It also supports the ability to save and load diagrams.

## Prerequisites
1. To run the program, [Python 3.9.1](https://www.python.org/downloads/) needs to be installed.
1. The program "ghostscript" must be installed on your machine. Downloads and installation instructions can be found here.
   https://www.ghostscript.com/download/gsdnld.html

   On Windows, you have to add ghostscript to your path. 
      * Press Windows Key + S to open the windows search bar (or click the search bar in the bottom left).
      * type "environment variables" into the search bar and press enter.
      * In the system properties menu that opens up, click "environment variables" near the bottom.
      * In the system variables section (lower half of window), double click on the row labled "Path"
      * In the edit environment variables window, click "new" on the right side.
      * In the new empty row created, paste the path to the installation of your ghostscript.
            Example path (64 bit) C:\Program Files\gs\gs9.54.0\bin\
   
      NOTE: On mac, the easiest way to install is to use homebrew.
      "brew install ghostscript"

1. During installation in Windows, check the box labeled "Add Python 3.9 to PATH" so Python programs can be run by typing `python` in a terminal.

## Package Installation
### Method 1 - No virtual environment
Assuming you are running [Python 3.9.1](https://www.python.org/downloads/) or later you can run `python -m pip install -r requirements.txt`. This will install all of the required packages to your system so you can run the program. If it fails however, move on to Method 2.

### Method 2 - Virtual environment using venv
If the installation script does not work for whatever reason, you can try running it within a virtual environment using `venv`
1. Invoke `python -m venv venv` within the project directory. This will create a new directory containing a python interpreter and `pip`.
1. To activate the virtual environment:

	On Windows (Powershell):
    
    	PS> venv\Scripts\Activate.ps1
    
    On MacOS/Linux:
    
    	$ source venv/bin/activate

1. Run `pip` to install the required packages by doing `python -m pip install -r requirements.txt`

## Running the program
1. Download the program from our [repository](https://github.com/mucsci-students/2021sp-420-MontyPython).
1. In a terminal, navigate to the directory the repository download has been saved in.
1. Follow one of the [package installation](#Package-Installation) guides.
1. If using a virtual environment, activate the environment (using step 2 from [package installation](#Package-Installation))
1. To run the program in GUI mode simply invoke `python Monty.py` within the root project directory. To run in CLI mode, add the `--cli` flag (`python Monty.py --cli`).
1. Follow the program’s prompts to create, load, or save a text representation of a UML diagram. Type `help` to view possible commands, or click `File > Help` in GUI mode.

### Example Images:  

#### CLI
![CLI](Images/cli.png)

#### GUI
![GUI](Images/gui.png)

## Authors
[Quinn Lehman](https://github.com/qlehman)

[Joseph Malone](https://github.com/jmalone35)

[Drew Tuckey](https://github.com/aptuckey)

[Sean Malloy](https://github.com/sfmalloy)

[Jen Hynes](https://github.com/Jen04)
