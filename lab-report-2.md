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
In the next example, the handleRequest method was called again after the user changed the URI parameter url to http://localhost:4000/add-messages?s=Nice!. This then output a string containing the current input, as well as retaining the information from the previous inputs. The returned value outputted: <br>
<br>
What day is it? <br>
Monday. <br>
Nice! <br>
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
