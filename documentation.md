# Start screen

![alt text](https://github.com/LizavetaVintsek/GPS-coordinates-converter/blob/master/GPS_converter_start_screen.png)

When the GPS coordinates converter application is just opened, all input and output fields are empty, the maps visualize the Kraków Old Town (the red marker has pinned to the localisation with the coordinates: 50.0612, 19.9377).
# The UI consists of three main parts:
1.	Convert coordinates from DD to DMS 
contains fields and buttons that allow user to convert coordinates from DD to DMS format, save converted coordinates, and reset the input fields
2.	Convert coordinates from DMS to DD
contains fields and buttons that allow user to convert coordinates from DMS to DD format, save converted coordinates, and reset the input fields
3.	Maps
contains the maps (Satellite and Normal Google maps) that visualise localisation corresponding to the converted coordinates

The application with valid input and output

![alt text](https://github.com/LizavetaVintsek/GPS-coordinates-converter/blob/master/GPS-converter_after_conversion.png)

# 1. The functionality of the ‘Convert coordinates from DD to DMS’ part:
1.1. Convert (DD to DMS part)
User can enter the DD latitude and longitude into the appropriate dark grey fields. Provided coordinates must contain only numbers, to separate whole and decimal numbers use the dot. The valid DD latitude must range from -90 to 90 (inclusive), the valid DD longitude must range from -180 to 180 (inclusive). After entering valid DD latitude and longitude click the ‘Convert DD to DMS’ button to convert the provided coordinates into the DMS format.
1.2. Save (DD to DMS part)
User can save the converted coordinates in both DD and DMS formats to the 'Saved coordinates.xlsx' file by pressing the 'Save to Excel' button. The confirmation message ‘Saved successfully’ will appear for 1.5 sec and will close automatically. To eliminate multiple savings of the same data, the 'Save to Excel' button will be disabled after the first press. To enable the 'Save to Excel' button, enter and convert new coordinates. The 'Saved coordinates.xlsx' must be closed during saving.

![alt text](https://github.com/LizavetaVintsek/GPS-coordinates-converter/blob/master/GPS_converter_save_confirmation_message.png)

1.3. Reset (DD to DMS part)
User can empty the DD latitude and DD longitude fields by clicking the ‘Reset’ button. The DD latitude and DD longitude fields can be also deleted/corrected manually by clicking on the appropriate fields and using a keyboard.

# 2. The functionality of the ‘Convert coordinates from DMS to DD’ part:
2.1. Convert (DMS to DD part) 
User can enter the DMS latitude and longitude into the appropriate dark grey fields. Provided coordinates must contain only numbers, except for the special characters (°, ', ") after degrees, minutes, and seconds, respectively (e.g. 11°31'45"). If the minutes and/or the seconds are absent in the coordinates write 0 (zero) instead (e.g. 11°0'0"). The valid DMS latitude degrees must range from 0 to 90 (inclusive). The valid DMS longitude degrees must range from 0 to 180 (inclusive). The valid DMS latitude/longitude minutes must range from 0 to 60 (inclusive). The valid DMS latitude/longitude seconds must range from 0 to 60 (inclusive). The user must select a direction radio buttons (N or S, and E or W). After entering valid DMS latitude and longitude and selecting direction click the ‘Convert DMS to DD’ button to convert the provided coordinates into the DD format.
2.2. Save (DMS to DD part)
User can save the converted coordinates in both DD and DMS formats to the 'Saved coordinates.xlsx' file by clicking the 'Save to Excel' button. The confirmation message ‘Saved successfully’ will appear for 1.5 sec and will close automatically. To eliminate multiple savings of the same data, the 'Save to Excel' button will be disabled after the first click. To enable the 'Save to Excel' button, enter and convert new coordinates. The 'Saved coordinates.xlsx' must be closed during saving.
2.3. Reset (DMS to DD part)
User can empty the DMS latitude and DMS longitude fields by clicking the ‘Reset’ button. The DMS latitude and DMS longitude fields can be also deleted/corrected manually by clicking on the appropriate fields and using a keyboard.

# 3. The functionality of the ‘Maps’ part:
3.1. When the user clicks the ‘Convert DD to DMS’ or ‘Convert DMS to DD’ buttons the area corresponding to the localisation of the converted coordinates will be visualized on both Satellite and Normal Google maps. The markers are placed directly on the localisation corresponding to the converted coordinates. User can change the zoom of the maps by clicking plus (‘+’) and minus (‘-‘) signs in the upper left corner of each map or using the mouse or touchpad. User can change the viewed area (left-right, up-down) using the mouse or touchpad.

# Pop-up messages

1.1. Pop-up messages in the Convert (DD to DMS part) functionality
1.1.1. If the user left the DD latitude field empty and clicks the ‘Convert DD to DMS’ button (valid DD longitude entered) the error message ‘Error: Please, enter the DD latitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
1.1.2. If the user enters into the DD latitude field any special characters (except for dot), and/or letters, and/or spaces (except for terminal spaces) and clicks the ‘Convert DD to DMS’ button (valid DD longitude entered) the error message 'Error: DD latitude should be a number!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
1.1.3. If the user enters the DD latitude that is less than -90 or greater than 90 and clicks the ‘Convert DD to DMS’ button (valid DD longitude entered) the error message 'Error: DD latitude should be between -90 and 90!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
1.1.4. If the user left the DD longitude field empty and clicks the ‘Convert DD to DMS’ button (valid DD latitude entered) the error message ‘Error: Please, enter the DD longitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
1.1.5. If the user enters into the DD longitude field any special characters (except for dot), letters, or spaces (except for terminal spaces) and clicks the ‘Convert DD to DMS’ button (valid DD latitude entered) the error message 'Error: DD longitude should be a number!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
1.1.6. If the user enters the DD longitude that is less than -180 or greater than 180 and clicks the ‘Convert DD to DMS’ button (valid DD latitude entered) the error message 'Error: DD longitude should be between -180 and 180!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.

1.2. Pop-up messages in the Save (DD to DMS part) functionality
1.2.1. If the user left the DD latitude field empty and clicks the ‘Save to Excel’ button the error message ‘Error: Please, enter the DD latitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
1.2.2. If the user left the DD longitude field empty and clicks the ‘Save to Excel’ button the error message ‘Error: Please, enter the DD longitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button. 
1.2.3. If the user enters the DD longitude and latitude but doesn’t convert it by clicking the ‘Convert DD to DMS’ button and clicks the ‘Save to Excel’ button the error message ‘Error: Please, convert the data!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
1.2.4. If the user tries to save previously saved converted coordinates by clicking again ‘Save to Excel’ button the error message ‘Convert new data to activate Save button’ will appear for 2 sec and will close automatically.

![alt text](https://github.com/LizavetaVintsek/GPS-coordinates-converter/blob/master/GPS_converter_save_error_message.png)

2.1. Pop-up messages in the Convert (DMS to DD part) functionality
2.1.1. If the user left the DMS latitude field empty and clicks the ‘Convert DMS to DD’ button (valid DMS longitude entered and all direction radio buttons selected) the error message ‘Error: Please, enter the DMS latitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.2. If the user enters into the DMS latitude field any special characters (except for one degree sign (°), one apostrophe (') and one single quotation mark (")), and/or letters, and clicks the ‘Convert DMS to DD’ button (valid DMS longitude entered and all direction radio buttons selected) the error message ‘Error: DMS latitude should contain only numbers!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.3. If the user enters the valid DMS latitude but adds some additional characters at the end (numbers, letters, special characters, spaces) and clicks the ‘Convert DMS to DD’ button (valid DMS longitude entered and all direction radio buttons selected)  the error message ‘Error: DMS latitude should be entered in the format DD°MM'SS"!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.4. If the user enters the DMS latitude degree that is less than 0 or greater than 90 and clicks the ‘Convert DMS to DD’ button (valid DMS longitude entered and all direction radio buttons selected) the error message ‘Error: Latitude degrees should be between 0 and 90!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.5. If the user enters the DMS latitude minutes that is less than 0 or greater than 60 and clicks the ‘Convert DMS to DD’ button (valid DMS longitude entered and all direction radio buttons selected) the error message ‘Error: Latitude minutes should be between 0 and 60!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.6. If the user enters the DMS latitude seconds that is less than 0 or greater than 60 and clicks the ‘Convert DMS to DD’ button (valid DMS longitude entered and all direction radio buttons selected) the error message ‘Error: Latitude seconds should be between 0 and 60!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.7. If the user left the DMS longitude field empty and clicks the ‘Convert DMS to DD’ button (valid DMS latitude entered and all direction radio buttons selected) the error message ‘Error: Please, enter the DMS longitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.8. If the user enters into the DMS longitude field any special characters (except for one degree sign (°), one apostrophe (') and one single quotation mark (")), and/or letters, and clicks the ‘Convert DMS to DD’ button (valid DMS latitude entered and all direction radio buttons selected) the error message ‘Error: DMS longitude should contain only numbers!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.9. If the user enters the valid DMS longitude but adds some additional characters at the end (numbers, letters, special characters, spaces) and clicks the ‘Convert DMS to DD’ button (valid DMS latitude entered and all direction radio buttons selected)  the error message ‘Error: DMS longitude should be entered in the format DD°MM'SS"!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.10. If the user enters the DMS longitude degree that is less than 0 or greater than 180 and clicks the ‘Convert DMS to DD’ button (valid DMS latitude entered and all direction radio buttons selected) the error message ‘Error: Longitude degrees should be between 0 and 180!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.11. If the user enters the DMS longitude minutes that is less than 0 or greater than 60 and clicks the ‘Convert DMS to DD’ button (valid DMS latitude entered and all direction radio buttons selected) the error message ‘Error: Longitude minutes should be between 0 and 60!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.1.12. If the user enters the DMS longitude seconds that is less than 0 or greater than 60 and clicks the ‘Convert DMS to DD’ button (valid DMS latitude entered and all direction radio buttons selected) the error message ‘Error: Longitude seconds should be between 0 and 60!' will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.

1.2. Pop-up messages in the Save (DD to DMS part) functionality
2.2.1. If the user left the DMS latitude field empty and clicks the ‘Save to Excel’ button the error message ‘Error: Please, enter the DMS latitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.2.2. If the user left the DMS longitude field empty and clicks the ‘Save to Excel’ button the error message ‘Error: Please, enter the DMS longitude value!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button. 
2.2.3. If the user enters the DMS longitude and latitude but doesn’t convert it by clicking the ‘Convert DMS to DD’ button and clicks the ‘Save to Excel’ button the error message ‘Error: Please, convert the data!’ will appear. The user can close the error message by clicking the ‘OK’ button or the close (cross) button.
2.2.4. If the user tries to save previously saved converted coordinates by clicking again ‘Save to Excel’ button the error message ‘Convert new data to activate Save button’ will appear for 2 sec and will close automatically.
