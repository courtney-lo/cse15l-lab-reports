## Week 5 Lab Report 3: Researching Commands
#### Find Command

##### Find -name
Example 1: <br>
<img src="https://user-images.githubusercontent.com/122492769/218555734-b30046c4-0923-4bd1-84f0-1b50dcae2afa.png" width="620" height="50"> 

Example 2: <br>
<img src="https://user-images.githubusercontent.com/122492769/218555816-4fc542a1-de59-4050-9d66-e765268d7eff.png" width="620" height="50"> 

In these examples I used the find -name command in order to find the file with the specific name in the specified directory to search, which in this case is the written_2 directory. This command is important as it can allow specific full pathways to be found for certain files, saving time and effort into looking for it individually.

##### Find -empty

Example 1: <br>
<img src="https://user-images.githubusercontent.com/122492769/218558619-1a926007-f315-4d58-aa93-7cda27203b1d.png" width="620" height="40"> 

Example 2: <br>
<img src="https://user-images.githubusercontent.com/122492769/218559072-892b09eb-9aa8-4f96-8486-8061333d4195.png" width="620" height="120"> 

In these examples I used the find -empty command to find the empty files within the specified directory, which was written_2. To show the output I first created an empty file called grep-results.txt, which was shown in the output of the first example since it was an empty file. However after removing the file, calling the find -empty command had no output, as all of the files within written_2 had some content in them. This is important as it can make sorting through files easier when wanting to remove excess files with no data or content in them, so people can clean their directories and file space.

Source: https://www.redhat.com/sysadmin/linux-find-command

##### Find -d

Example 1: <br>
<img src="https://user-images.githubusercontent.com/122492769/218564492-09c9c1c2-c3bc-41a7-ae81-c01c3bca918c.png" width="375" height="600"> 

Example 2: <br>
<img src="https://user-images.githubusercontent.com/122492769/218564505-a26a2f82-b5c5-4a2f-9971-8714df2215f1.png" width="375" height="600"> 

In these examples I used the find -d command which lists all the files and directories in the specified directory. This is important to know so that users can see everything that is in the current directory they are looking in. This command can then be used to sort through or filter through different files in a specific directory.

Source: https://www.tecmint.com/35-practical-examples-of-linux-find-command/

##### Find -type f

Example 1: <br>
<img src="https://user-images.githubusercontent.com/122492769/218574731-47384b4b-fa2b-4f05-868b-7148b8e891d4.png" width="500" height="600"> 

Example 2: <br>
<img src="https://user-images.githubusercontent.com/122492769/218574753-bf31c33c-75ba-42b5-acc9-47c63472bf9f.png" width="500" height="600"> 

In these examples, I used the find -type f command. F stands for file and the -type command goes through everything in the current directory and prints out the ones that match the following type that the user specifies in the linux command. In the first example, I wanted to print out all of the files in the directory written_2, so I used the -type f command. Another option is the -type d, where d stands for directories. This is an important command to know because it easily outputs all of the files or directories of the user's choice, so that no extra filtering or commands are needed.
