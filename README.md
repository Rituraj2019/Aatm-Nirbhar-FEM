# IITR_CMLab
Project of Summer Internship'22 | CMLab, IIT Roorkee
## Files
**main.py**: This is a python file to run our application/GUI. This file runs using different modules made in @modules file

**modules**: These are different python modules which are imported in main.py for working of GUI

**main.ui**: Qt designer file. This is made inside Qt creator/designer. The exported file generates .ui file which is then converted to .py file. ui_main.py is the python file converted from this .ui file.

**themes**: This file contains different themes for out GUI

**images**: This file contains different images used in making of our GUI

**dist**: This file contains the executable(.exe) form of our GUI. 

**icon.ico**: This is a central icon of our project

**modules/ui_functions.py**: Functions related to GUI

**modules/ui_main.py**: Qt designer exports .ui file which contains xml code. To make xml code editable we convert that to .py file using **pyuic6 -o output.py -x input.ui**   Here, pyuic6 is because we are using pyqt6. -o is followed by python file we want to get output as. And -x is followed by input file which is in .ui file.

## Process to convert .py to .exe
Step1: In CMD: **pip install pyinstaller**

Step2: In project directory(make sure all the necessary files are in this directory): **pyinstaller --onefile -w filename.py** ,(filename.py=main.py in our case). This will create some files in project directory

Step3: Open dist file to get executable(.exe) file for use

## Process to convert .ui file of Qt to editable .py file
.ui file is xml file and we can’t modify that to our need. We therefore convert this .ui file to .py file and modify according to our need. 
To modify, 

Step1: Open cmd at the .ui file location. (UI file will be created inside the project folder)

Step2: Now inside cmd use: **pyuic6 -o output.py -x input.ui**    
       Here, pyuic6 is because we are using pyqt6. -o is followed by python file we want to get output as. And -x is followed by input file which is in .ui file.
       
Step3: Open project file, .py file will be available as (output.py)


