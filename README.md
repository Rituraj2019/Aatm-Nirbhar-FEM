# IITR_CMLab
Project of Summer Internship 2022 | CMLab, IIT Roorkee
## Files
**main.py**: This is a python file to run our application/GUI. This file runs using different modules made in @modules file

**modules**: These are different python modules which are imported in main.py for working of GUI

**main.ui**: Qt designer file. This is made inside Qt creator/designer. The exported file generates .ui file which is then converted to .py file. @ui_main.py is the python file converted from this .ui file.

**themes**: This file contains different themes for our GUI

**images**: This file contains different images used in making of our GUI

**dist**: This file contains the executable(.exe) form of our GUI. 

**icon.ico**: This is a central icon of our project

**modules/ui_functions.py**: Functions related to GUI

**modules/app_functions.py**: Some additional function to manually change style of some widgets. qss unfortunately suffers inheritance problem where they end up inheriting styles from their parents. Using this funtion we have created hacks for these functions of selecting menu buttons (in left side of UI) and also functions related to buttons present in right of UI is added here.

**modules/ui_main.py**: Qt designer exports .ui file which contains xml code. To make xml code editable and accessible we convert that to .py file using **pyside6-uic input.ui -o output.py**. 

**.idea** and **pycache**: These are auto created files during making python project directory for our project in pycharm. These files are not necessary in making of our project

**resources.qrc**: Resources used for Qt designer. Add here using Qt designer

## Process to convert .py to .exe
Step1: In CMD: **pip install pyinstaller**

Step2: In project directory(make sure all the necessary files are in this directory): **pyinstaller --onefile -w filename.py** ,(filename.py=main.py in our case). This will create some files in project directory

Step3: Open dist file to get executable(.exe) file for use

## Process to convert .ui file of Qt to editable .py file
.ui file is xml file and we can’t modify that to our need. We therefore convert this .ui file to .py file and modify according to our need. 
To modify, 

Step1: Open cmd at the .ui file location. (UI file will be created inside the project folder)

Step2: Now inside cmd use: **pyside6-uic input.ui -o output.py*
       
Step3: Open project file, .py file will be available as (output.py)


