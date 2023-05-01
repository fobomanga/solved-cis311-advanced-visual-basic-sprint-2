Download Link: https://assignmentchef.com/product/solved-cis311-advanced-visual-basic-sprint-2
<br>
<h1></h1>

Agile programmers refer to code that doesn’t look right as having a “smell”. Some of the features that make a piece of code smell are poor documentation, variable names that are not descriptive, and code that is repeated. By now you should be able to sense that the code for Airports definitely has a smell. Unless something is done to take care of the smell, it will build up a technical debt. The greater the technical debt, the more difficult it will be in the future to make improvements to the code. This eventually can lead to a situation where any changes to the code cause more problems than they cure.

In CIS310 we emphasized the importance of good documentation and good variable names, but the main offender in this code is the repetition. The cure for repetition is refactoring (specifically Extraction), which just means extracting common code and placing it in a procedure, preferably a function. Then, wherever that code was used, replace it with a call to the new function.

This sprint will be particularly challenging because of the interconnectedness of all your code. At times you will have to wait to test your code until other members of your team have finished theirs, so be sure to communicate your progress in your daily scrum meeting. Next week we will introduce a solution that makes it much easier to work around each other when working on the same code.  Since there are more tasks than team members, some of you will have the opportunity of completing more than one task.




Story:    As a system administrator, I want the code for the distance calculator program to be refactored for easier maintenance.




Task 1:  Create a function named CoordinateToDegrees to refactor the code that converts a latitude or longitude into a value in decimal degrees. (This function will be used inside the function Distance.)

Task 1a:    Write the code for the CoordinateToDegrees function with an input parameter for DegreeString as type string, and returns the value in decimal Degrees as type Double. The stub for this function has been provided.

Task 1b:    Check out the master copy of the project and install your changes. Testing will be done by the team member in charge of task 4.




Task 2:  Create a function named DegreesToRadians to refactor the code that converts a latitude or longitude in decimal degrees to a value in radians. (This function will be used inside the function Distance.)

Task 2a:    Write the code for the DegreesToRadians function with an input parameter for DegreesDouble as type double, and returns the value Radians as type Double. The stub for this function has been provided.

Task 2b:    Check out the master copy of the project and install your changes. Testing will be done by the team member in charge of task 4.




Task3:   Create a function named ValueOf to refactor the code that translates a selected index into a related string (city, latitude, or longitude).

Task 3a:    Write the code for the ValueOf function with input parameters for Index as type Integer, which identifies the record in the array Hubs, and FieldName as type FieldNames (an enumeration that has been provided), which identifies which field in the Airport structure to return. The function ValueOf returns the value indicated as type string. The stub for this function has been provided.

Task 3b:    Check out the master copy of the project and install your changes. Testing will be done by the team member in charge of task 5.




Task 4:  Create a function named Distance to refactor the code that calculates the shortest distance in miles between two points on the earth. Replace the code for the CalcDistanceButton event to use the results returned by the function Distance.

Task 4a:    After the completion of task 1 and 2 write the code for the Distance function with input parameters for the indexes of two cities, Index1 and Index2, as type integer, and returns the distance in miles between the two cities as type Double. Use the functions CoordinateToDegrees and DegreesToRadians to convert the latitudes and longitudes in Hubs for Index1 and Index2 to radians for the calculation. The stub for this function has been provided.

Task 4b:    Rewrite the code for the CalcDistanceButton_Click event to use the function Distance to fill the associated textbox, DistanceTextBox.

Task 4c:    Test the CalcDistanceButton to assure that the distance between Atlanta and Boston displays as 945 miles.

Task 4d:    Check out the master copy of the project and install your changes.




Task 5:  Replace the code for the two ComboBox events to use the results returned by the function ValueOf.

Task 3a:    After the completion of task 3, rewrite the code for the ComboBox events, ID1ComboBox_Selected and ID2ComboBox_Selected, to use the function ValueOf to fill the associated TextBoxes.

Task3b:     Test each ComboBox, to assure that Atlanta’s latitude displays as 33°38’22”.

Task3c:     Check out the master copy of the project and install your changes.




Task 6: Remove the Calc Buttons from the Form.

Task 6a:    After the completion of task 4, remove the Calc1Button and Calc2Button controls. They were Jetson buttons<a href="#_ftn1" name="_ftnref1">[1]</a> and no longer serve any purpose.

Task 6b:    Check out the master copy of the project and install your changes. Testing will be done by the team member in charge of task 7.




Task 7: Do a final check and publish results in the Weekly Discussion Board.

Task 7a:    Check out the master copy of the project and test each Control on the form to assure that Atlanta’s latitude displays as 33°38’22” and the distance between Atlanta and Boston displays as 945 miles.

Task 7b:    On Wednesday, after the completion of all other tasks, insert the most recent copy of AirportDistances.exe in the Weekly Discussion Board for your team.




<a href="#_ftnref1" name="_ftn1">[1]</a> George Jetson was the star of a cartoon called The Jetsons. He worked at Spacely Sprockets, where his occupation was to push the on/off button for the otherwise completely automated factory.