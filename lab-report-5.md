## Week 9 Lab Report 5

#### Part 1: Lab Report 3 Using Find Command

My favorite lab report that I did this quarter was lab report 3, which was the exploration of different ways you can execute a certain command. I chose to use the find command, as that was the one command that I felt would be the most useful to me going forward in the course, however, I do wish that I took the time to learn more about other commands, which is why I chose this lab report to relook at.

##### How I did the task:

I began by searching up different ways to use the find command – looking for directories, empty files, names of files, etc. – and used a cloned repository to test the outputs of the commands in the terminal. I also cited each of the websites that I learned the command from or learned more in-depth about what the command does. Finally I wrote descriptions of the output of each of the commands, as well as what it was doing to the directories, providing images to visualize the outputs.

##### Going forward:

In this lab I hope to research more about other commands, such remove (rm), so that I can get a better understanding of different terminal commands I can call to manipulate and navigate my directories and files.

#### Part 2: The Lab with Remove Command

##### rm -fv

Example 1:

current .txt files –

<img width="662" alt="Screenshot 2023-03-13 at 3 31 28 PM" src="https://user-images.githubusercontent.com/122492769/224848331-de52d73e-6cfb-479f-ad4c-e090e38d57c7.png">

after calling rm -fv –

<img width="612" alt="Screenshot 2023-03-13 at 3 32 36 PM" src="https://user-images.githubusercontent.com/122492769/224848338-459c9886-a9c0-4d82-9c50-d10355a77d1a.png">

Example 2:

current .txt files –

<img width="641" alt="Screenshot 2023-03-13 at 3 39 10 PM" src="https://user-images.githubusercontent.com/122492769/224848352-4ed71e07-92a0-40a8-8b2d-863c233f237c.png">

after calling rm -fv –

<img width="559" alt="Screenshot 2023-03-13 at 3 40 52 PM" src="https://user-images.githubusercontent.com/122492769/224848491-4809377e-6b36-49eb-a2b0-195a93276f1b.png">


In these examples, I used the remove -fv command to remove all .txt files in the current directory without getting a prompt or warning message. This command is important because we learned about how to find all the .txt files in the current directory, but in the case we want to remove them, rather than spending time removing each file individually, we can just use this command. It ultimately saves a lot of time and effort.


##### rm -i

Example 1: Confirming yes to removing the file

<img width="379" alt="Screenshot 2023-03-13 at 3 45 52 PM" src="https://user-images.githubusercontent.com/122492769/224849545-93371c6c-a77e-4295-befb-4a72411ac4f6.png">

Example 2: Saying no to removing the file

<img width="386" alt="Screenshot 2023-03-13 at 3 46 31 PM" src="https://user-images.githubusercontent.com/122492769/224849583-418327b6-7d96-4003-a89d-a596ab98ae37.png">

In these examples, I used the remove -i command in order to have a confirmation message pop up, prompting me to confirm each file I call to remove. This is an important command in case the user makes a mistake and doesn't mean to remove the file they called the command to remove. It prevents the user from making careless mistakes and losing files that are needed.

##### rm -d

Example 1:

<img width="649" alt="Screenshot 2023-03-13 at 3 49 46 PM" src="https://user-images.githubusercontent.com/122492769/224849815-2876a4ee-c6bc-464a-9fbe-3840f6f947f6.png">

Example 2:

<img width="458" alt="Screenshot 2023-03-13 at 3 50 13 PM" src="https://user-images.githubusercontent.com/122492769/224849841-0dd88327-8fa9-447b-b73e-09b8339f4c26.png">

In these examples, I used the remove -d command in order to remove an empty directory rather than just files within the directory. This is an important command as it can be used to keep the user's system clean and organized. Empty directories may clutter the interface, and so it is important to have a command to remove these directories in order to keep a clean work environment.

##### rm -r

Example 1:

<img width="1049" alt="Screenshot 2023-03-13 at 3 35 26 PM" src="https://user-images.githubusercontent.com/122492769/224847697-d5418b06-3d48-426a-ad63-6a55e20c1359.png">

Example 2:

<img width="457" alt="Screenshot 2023-03-13 at 3 42 16 PM" src="https://user-images.githubusercontent.com/122492769/224848718-1cad7b88-bd1c-422c-9ef4-083696ffebae.png">

In these examples, I used the remove -r command in order to remove non-empty directories. The command recursively passes through all the files within the directory, removing them, and then finally removing the directory itself. This is ipmortant becaues it allows us to remove directories that contain files we no logner need before, clearing up cluttered systems, and saving time and effort from having to call multiple commands.


