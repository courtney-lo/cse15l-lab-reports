## Week 3 Lab Report 2: Servers and Bugs
#### Step 1: StringServer
Code for StringServer is shown below:

<img src="https://user-images.githubusercontent.com/122492769/215405868-c064c86a-cc64-4d4c-a58b-2ac794c59e3c.png" width="500" height="350"> 

Example 1: <br>
In the example below, the handleRequest method was called, which takes in a URI called url as the parameter and returns a String of all the inputs. The parameter taken in is broken apart using the .split() method which separates the non-changing part of the url, with the user changed part. In this case, the URI parameter url input was originally http://localhost:4000/add-messages?s=What%20day%20is%20it?, which outputted the string: <br>
<br>
What day is it? <br>
<br>
The url was then changed by the user to http://localhost:4000/add-messages?s=Monday., which changed the output to return: <br>
<br>
What day is it? <br>
Monday. <br>

<img src="https://user-images.githubusercontent.com/122492769/215407508-6a6357bb-3f56-4e95-872e-253694fde05f.png" width="700" height="200"> 



Example 2:
