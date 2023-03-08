# GPS-coordinates-converter

## Installation

The application is built using Tkinter which is Python's standard GUI (Graphical User Interface) package. The application is offline and can be used only after downloading the GPS-converter.py and logo-gps.ico files on the user's computer. User must have preinstalled Python and Python interpreter (the application is created using Python 3.10.4 and PyCharm Edu 2021.3.2 as an interpreter). The stability of the application using other versions of Python and other interpreters is not tested. To open the application the user must open GPS-converter.py file in the Python interpreter and run it. Additional packages that must be installed are openpyxl, xlrd, pathlib2, tkintermapview, customtkinter.

## The program allows you:
- to convert GPS coordinates from DD (decimal degrees) format to DMS (degrees, minutes, seconds) format and vice versa; 
- to save converted coordinates in both formats to the .xlsx file;
- to visualise localisation that corresponds to converted coordinates on the maps (Satellite and Normal Google maps).

![alt text](https://github.com/LizavetaVintsek/GPS-coordinates-converter/blob/master/UI_images/GPS_converter_start_screen.png)

To convert coordinates:
1. Enter the latitude and longitude in the appropriate fields. While converting DMS to DD coordinates, choose the direction (N or S, E or W).
2. Press the 'Convert' button. Localisation that corresponds to converted coordinates will be automatically shown on the maps.
Notes: 
1. The coordinates in DD format should contain only numbers. Use a dot to separate whole and decimal numbers (ex. 45.9876).
2. The coordinates in DMS format should contain only numbers. Use special characters (°, ', ") after degrees, minutes, and seconds, respectively (ex. 11°31'45"). 

To save converted coordinates to the 'Saved coordinates.xlsx' file press the 'Save to Excel' button. To eliminate multiple savings of the same data, the 'Save to Excel' button will be disabled after the first press. To enable the 'Save to Excel' button, enter and convert new coordinates.

To enter new coordinates you can:
- use the 'Reset' button, to delete data from all fields and then enter the coordinates into the input fields manually, or 
- change the input fields manually using a keyboard.


**The complete documentation is stored in the documentation.md file.** 

**The user story, test cases (Zephyr Scale) and bug reports are in Jira under the link below**

*https://lizavetavintsek.atlassian.net/jira/software/c/projects/CCT/boards/2/backlog?issueLimit=100*
