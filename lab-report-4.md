## Week 7 Lab Report 4

#### Step 4: Log into ien6 account

Key's pressed: ```<up><enter>```

<img width="532" alt="Screenshot 2023-02-27 at 5 42 46 PM" src="https://user-images.githubusercontent.com/122492769/221731499-feaa7568-c78e-4dea-8dde-73857ea14c88.png">

I pressed the ```<up>``` key in my terminal in order to call the most previous line that I entered into my terminal, which was 
  ``` ssh cs15lwi23abz@ieng6.ucsd.edu. ```
By pressing ```<enter>``` I was able to log into my ien6 account.

#### Step 5: Clone your fork of the repository from your Github account

Key's pressed: ```<Ctrl-C> <Ctrl-V> <enter>```

<img width="722" alt="Screenshot 2023-02-27 at 5 50 20 PM" src="https://user-images.githubusercontent.com/122492769/221732176-cb984c79-b519-4d90-8c4f-e89592ecec3e.png">

I first used ```<Ctrl-C>``` to copy the SSH url from github of my forked lab7 repository. I then used ```<Ctrl-V>``` to paste the SSH url after the command git clone in order to clone the forked repository onto my SSH remote-computer account. Finally, in order to run all the commands I pressed ```<enter>```, which ran 
  ``` git clone git@github.com:courtney-lo/lab7.git ```

#### Step 6: Run the tests, demonstrating that they fail

Key's pressed: ``` <Ctrl-C> <Ctrl-V> <enter> <Ctrl_C> <Ctrl-V> <Ctrl-C> <Ctrl-V> <enter> ```

<img width="652" alt="Screenshot 2023-02-27 at 6 00 01 PM" src="https://user-images.githubusercontent.com/122492769/221733510-6fbd2e41-1192-4131-9971-a2dfc0068388.png">

In order to run the tests within the lab7 repository, I first had to switch into the lab7 directory using ```cd lab7```. I used ```<Ctrl-C>``` to copy the two JUnit commands and name of the tester file (ListExamplesTest.java) and then used  ```Ctrl-V``` to paste the commands into my terminal as shown below: <br>
```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java ``` <br>
```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTest.java```<br>
In order to run both of these commands, I used ```<enter>```.
