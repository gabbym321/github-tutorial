# GitHub Tutorial

by Gabriel Makower 

---
## Git vs. GitHub
#### Git:   
 
Git is a software that runs in the command line. Git takes a snapshot of code that you write so you can look back at it. Git also allows you to send things up to your remote repository (the cloud) and to pull it back down.   

#### Github:   
 
GitHub is a web-based git respotory hosting service, you may often hear this being referd to as the cloud. Github is different to git beause you will always need git for github but you may not always need github for git. Github is an amayzing tool because it provides a easy way to colaborate your code with someone else. Because it is on the internet anyone can see it and pull it down to their local repository so that they can make changes to it that you have the ability to accept or deny.  


---
## Initial Setup
###### Now that you know the basic idea of git and github, its time to put them into use.
1) First we need to make a Cloud 9 account. Go to c9.io and click on sign up. Fill out all the information and make sure you use an email that you have access to. 

2) Now we make a github account. Go to github.com and fill out all the information. **_When you are done make sure you go back to your email and verfy with github!_**

3) Now we have to link our local (_c9_) to our remote (_github_) to do this you need to go to c9 and click the settings icon in the top right corner. in the settings click connected services and look for github. Click connect. 

4) Now that you connected c9 to github, we need to make a workspace in our c9 so we can start coding. To do this click the + create new workspace. Name your workspace and put a discription. Dont set a team and make the workspace blank. Now click create workspace.  




---
## Repository Setup
###### Now we can start coding!  

1)  First thing we need to do is get into our master directory. To get into any directory or repository we have `cd` into it we use a tilde (~) to tell the computer anywhere you are, go into the directory that I am telling you to go in. For example, if I choose to make my first repo in the directory workspace, I would type in this: `cd ~/workspace`. 

2) Now that we are in our workspace, we can make our first repo. to make a repository you first need to make a directory. type the code `mkdir` then then name you want your directory (or soon to be repository) to be called. in this example I'll call this first-repo. So I would type `mkdir first-repo` 

3) Now that we made a new directory, we need to initialize git so that our directory turns into a repository and we can do things like send our work up to the cloud (Github). to do this, we type in the command `git init` this will "hire" git so you can start using it. _You only have to do this once._

4) Now you want to make a connection from your git to github. to do this go on git and press the add button on the top right. then click _new repository_. Type in the repository name that you made in your local. Now click create repository. You now have a connection between your local and remote. 


4) We have a repo and git initialized so now lets make a file that we can type information into. to make a file you type in `touch <file.name>` Now click on the file you made. you will see it on the left. now you can type what ever you want into that file. 

5) Now that we have the file we want to add it to the staging area. to do this type in your repository `git add .` 

6) Now to check if the file has been added type `git status` you should see something in green. that means your file is tracked and on the staging area.  

7) Now we can move onto the next step which is commiting the file. This tells git to actually take the "snapshot" of the file. to do this type `git commit -m` "_small meassege about what you are commiting_" make sure in the meassege you dont use past tense and you make it short and to the point.
* _A common mistake is to forget to put the -m after commit. If this happens you might see a weird message. all you have to do to get out of it is press command X_
* _another mistake people make is forgetting to put a quotation mark after the message. if you do this you will see a `>` to get rid of this press command c_

8) Now we can finally push it up to our remote repo (_github_) so that it can save on the internet for everyone to see. to do this type `git push -u orgin master` then check github to make sure you see your file. 




---
## Workflow & Commands
###### Now that we set up, we need to get into a consistent work flow. here is what we do everytime we start working. 

1) The first step is to go into your repo. to do this we type `cd repo-name` you type what ever your repository name is after `cd` 

2) Now we can edit our files. Type what ever you want into your files but every so often we want to add, commit and push it just incase something happens to our local repo. We want everything in the cloud. 

3) Everytime you finish a chunk of work follow this procedure. fist you type in `git add .` this puts your file in the frame of your staging area. 


4) Now you should check if its tracked in the staging area. To do this type `git status`. You should see writing in green. 

5) now you need to commit your work. to do this type `git commit -m "_short message_"

6) Now its time to push it up to the cloud. because when you were setting everything up you put `-u orgin master` all you need to type now is `git push` this send everything up to the cloud. 
* _A common mistake people make is trying to push their repository. Make sure you are only push a file. Redo it if you accedently put the repo._
7) now you can continue typing in your file and when you finish a chunck repeate steps 3-6. 



