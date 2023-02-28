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

#### Step 7: Edit the code file to fix the failing test

The error was in the last while loop which incremented the wrong variable ```index1``` instead of ```index2``` as it was looping through ```list2``` not ```list1```.

<img width="704" alt="Screenshot 2023-02-27 at 6 18 41 PM" src="https://user-images.githubusercontent.com/122492769/221738539-6152e0d6-5917-438c-a1a6-3c1cee15f7b1.png">

Key's pressed: ```<right>``` x 7, ```<Ctrl-O> <Ctrl-X>``` 

I used the right arrow key to move my cursor over the code in order to get to the line that I wanted to fix, after fixing I used ```<Ctrl-O>``` to save the changes and ```<Ctrl-X>``` to exit out of nano.

#### Step 8: Run the tests, demonstrating that they now succeed

Key's pressed: ```<up>``` x 2, ```<enter>```, ```<up>``` x 2, ```<enter>```

<img width="978" alt="Screenshot 2023-02-27 at 6 33 34 PM" src="https://user-images.githubusercontent.com/122492769/221739558-0574bf0a-c2a9-41b1-89ba-4f3923f3d7e4.png">

In order to run the tests, I used ```<up>``` (up arrow key) to use a line that I called earlier in the terminal, and I used ```<enter>``` in order to run the terminal command, which I repeated for both JUnit linux test commands: <br>
```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java ``` <br>
```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTest.java```<br>

#### Step 9: Commit and push the resulting change to your Github account

Key's pressed: ```<tab> <enter>```

<img width="785" alt="Screenshot 2023-02-27 at 6 48 32 PM" src="https://user-images.githubusercontent.com/122492769/221740725-9faa6bd5-55ac-400c-a0a0-6205eb424874.png">

I used ```git add ListExamples.java``` and ```git commit -m "updated code"``` to account for the changed code in the files due to the error correction, and then used ```git push``` in order to push the changes to the forked repository on GitHub. I used the ```<tab>``` key in order to finsih words that I didn't want to type out, for example: ```Li<tab>.java``` in order to complete the phrase ListExamples.java for the ```git add ListExamples.java``` command. I also used ```<enter>``` in order to run each of the commands.
