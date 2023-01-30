## Week 3 Lab Report 2: Servers and Bugs
#### Step 1: StringServer
Code for StringServer is shown below:

<img src="https://user-images.githubusercontent.com/122492769/215405868-c064c86a-cc64-4d4c-a58b-2ac794c59e3c.png" width="500" height="350"> 

Example 1: <br>
In the example below, the handleRequest method was called, which takes in a URI called url as the parameter and returns a String of all the inputs. The parameter taken in is broken apart using the .split() method which separates the non-changing part of the url, with the user changed part. In this case, the URI parameter url input was originally http://localhost:4000/add-messages?s=What%20day%20is%20it?, which outputted the string: <br>
<br>
*What day is it?* <br>
<br>
The url was then changed by the user to http://localhost:4000/add-messages?s=Monday., which changed the output to return: <br>
<br>
*What day is it?* <br>
*Monday.* <br>

<img src="https://user-images.githubusercontent.com/122492769/215407508-6a6357bb-3f56-4e95-872e-253694fde05f.png" width="700" height="200"> 



Example 2:
In the next example, the handleRequest method was called again after the user changed the URI parameter url to http://localhost:4000/add-messages?s=Nice!. This then output a string containing the current input, as well as retaining the information from the previous inputs. The returned value outputted: <br>
<br>
*What day is it?* <br>
*Monday.* <br>
*Nice!* <br>
<br>

<img src="https://user-images.githubusercontent.com/122492769/215408296-a125d116-f00c-41ea-ba90-2062f5c14307.png" width="700" height="200"> 

#### Step 2: Bugs

Failure-inducting test input and code:

```java
 public void testAverageWithoutLowest() {
    double[] input1 = { -1, -1, 0, 1, 2};
    double average = ArrayExamples.averageWithoutLowest(input1);
    assertEquals(1.0, average, 0.0);
 }
```

Non-failure inducing test input and code:

```java
 public void testAverageWithoutLowest() {
    double[] input2 = {0, 1, 2, 3};
    double average2 = ArrayExamples.averageWithoutLowest(input2);
    assertEquals(2, average2, 0.0);
 }
```

Symptom of code after running two JUnit test inputs:
<br>
<img src="https://user-images.githubusercontent.com/122492769/215606753-c73c7c23-349e-4145-b91d-a1a42e6cdf11.png" width="600" height="450"> 
<br>

Original code that contains a bug:

```java
  static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
  }
  ```

Changed code that fixed the bug:
```java
  static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    double count = 0;
    for(double num: arr) {
      if(num != lowest) { 
        sum += num; 
        count++;
      }
    }
    return sum / count;
  }
  ```
<br>
In the original code, the average does not account for there to be repeats of the same number in the array. This causes the calculated average without the lowest number to be incorrect when repeats of the lowest number occur. This is because more than one int in the array is not being added to the sum, but the dividing number is fixed to always be one less than the length of the array. To fix this, a count must be implemented to account for how many elements of the array are being added to the sum, so that the average will be calculated correctly, even if multiple elements aren't being used.
<br>
<br>
Below shows the test cases after the changes in the code are made:
<br>
<img src="https://user-images.githubusercontent.com/122492769/215609741-5edab7eb-364b-4051-9842-741f0a94e4ca.png" width="650" height="400"> 

#### Step 3: What I Learned
During week 2 and week 3 of lab, I learned how to implement a simple web server. Before this lab I was unaware of what a port number was, or how websites knew what to do based off of different commands to the query. I learned how methods such as the .contains() method can be used to check what the path is implementing, in this case checking for any added messages from the user. As well as learned how the .split() method can be used to get the user's input and return it on the web server.
