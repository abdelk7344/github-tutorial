# GitHub Tutorial

_by Abdelmonem Khedr_

---
## Git vs. GitHub
* Git allows us to take "snapshots" of our code and does not require the use of github
* Github requires git to function and takes these snapshots and stores them in the cloud (a website) 


---
## Initial Setup  
#### Github Account 
1. Click the Sign Up botton and enter a username, email, and a password. Select a free account. 
2. Click the top right icon and go to settings,then go to SSH and GPG keys in personal settings.
3. Copy the SSH key from github,then go to c9 and click on the gear icon on the top right.
4. Paste the SSH key in the box.
5. Go to your IDE (cloud 9) and press the gear icon . Go to _Connected Services_ and as you see github press connect.

--- 
#### SHS Key
1. To make an SSH key go first to [github.com](github.com) and log in
2. On the top right, click on your profile icon and press settings 
3. On the left side bar, click "SHSS and GPG Keys"
4. Create a new SHS key and give it a specfic and informtive title 
5. Get the SHS key from IDE. They usually starts with **shs-sa**. _( if using cloud9 then go to top right gear icon and press SHS key tab )_
6. Paste your SHS into github and press _Add SHS_ key
7. Go to your IDE and type `shs -T git@github.com` ( you should get a message stating your username and some type of approval message )


---
## Repository Setup
1. Go to your IDE and create a new foleder by typing `mkdir (foldername)`
2. Intialzes git in that directory to make it a repository. You can do this by typing `git init`
3. `cd` into that folder and create a "readme" file by typing `touch README.md`
4. Open your file by clicking on it _(if you are in cloud 9 you can type `c9 (filename)` to open it directly)_
5. Type a message in that file but make it relevant
6. Add this file to the staging area by typing `git add README.md` or `git add .`
7. Commit this change by typing in `commit -m "(type here a specfic and informitive message to what you did to your file)"`
8. Open a new tap and go to [github.com](github.com). Go to the top right corner and press the plus sign and in the drop down menu click _New Repository_
9. **(Important!)** **Give your repository name the same name you gave your repository in your IDE**
10. Click on *SHS* _(the tab next to **https**)_ and under where it says _"or push and existing an existing repository from the command line"_, copy each line one at a time and paste it in your IDE
11. You have know connected your local repo to the cloud 

---
## Workflow & Commands
1. Once you have made a change to your file, you have to make sure its is saved 
2. Type in `git status` and you should see that your file as of now is untracked(red)
3. Type `git add .` to add all file changes or type in `git add (filename)` just to add the changes for a specific file 
4. Again type in `git status` and you should see that your file is now in the staging area(green)
5. You can now commit a file by typing `git commit -m "(specific message)"` and you should write **a specific message to demonstrate what changes have been made**
6. Know that you have a commit you can know push the changes up to the cloud. Type `git push` and you should see that your changes should have been pushed by going to [github.com](github.com) and clicking on your repo
7. If `git push` did not work than most likely you didn't do the intial setup first (refer to _Intial Setup_)
8. Always use **`git status`** . It tells you alot about where your files are and if they are ready to be commited or pushed 

---
## Error Handeling 
* If you type `git init` in the wrong dicrtory and intialize git, type `rm -rf.git` to unintialize git from the current direcctroy that you are in 
* If in any case you want to delete your repo(local and remote)
  1. Go to your IDE and in your repo type in `rm -rf.git` and this will delete your local
  2. Go to github and click your repo. Click _setting_ and go all they way down till you see **Delete this Repository** and go ahead and press delete and type the name of your repo. You have delted your remote.

--- 
## Collaboration
1. Go to the repository that you will be , after cloning, making modifications on 
2. Click **Fork** on the top right under your icon
3. After you **Fork** it, press the green **Clone or Download** button
4. If its not already clicked of _SHS_ then click _SHS_
5. Grap the url given to you and clone it in your IDE by typing `git clone (url)`
6. `cd` in to that repo and make your modifications 
7. Add file by typing `git add .` or `git add (filename)`
8. Commit it by typing `git commit -m (write a specific message on the change you made)`
9. Write in `git push` after you have commmit your file. This will send it up to github.
10. To make a pull go to **your** forked repo on github and press _New pull request_ and type in a brief messgae on what you modified and send
11. If the owner thinks the modifications were needed or beneficial he or she can accept the request or in other cases deny it
12. If the owner accepts the pull request, they will have to return to their IDE and go into the repo and type in `git pull`. This will ensure that the changes are also on their local. 
