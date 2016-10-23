# GitHub Tutorial

_by Abdelmonem Khedr_

---
## Git vs. GitHub
* Git allows us to take a "snapshot" of our code and does not require the use of github
* Github requires git and takes these snapshots and stores them in the cloud (a website) 


---
## Initial Setup
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
9. **Give your repository name the same name you gave your repository in your IDE**
10. Click on *SHS* _(the tab next to **https**)_ and under where it says _"or push and existing an existing repository from the command line"_, copy each line one at a time and paste it in your IDE
11. You have know connected your local repo to the cloud 

---
## Workflow & Commands