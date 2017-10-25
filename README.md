# GitHub Tutorial

_By: Anabel Arbeeny_

---
## Git vs. GitHub
#### Git-  
Git is used to store "screencshots" of code so that you have "checkpoints" of code so if the code breaks you have somewhere to go back to and start fresh.Git does not require git hub to work. Git uses commands:


#### GitHub-  
[GitHub](www.github.com) is a cloud that when you push the "screenshot" it is held there and you can acess it anywhere. Github allows for easier collaboration between coders because it stores the repositories 

---
## Initial Setup
**_Intial Setup_**- When you want to use git and github you need to create your profiles one on github and one for your local repo unless you have 
### setting up an account for GitHub 
* 1- The first step it to got to [github](www.github.com)
* 2- Now you are on the home page in the top right corner you will see "sign up" click that and follow the instructions 
(include how to sign into c9.io)


* 3- After you setup the Github account look around and become familiar with GitHubs setup and what the website is like. 

### Setting up c9.io
* 1- Go to [Cloud9](https://c9.io) 
* 2- In the top right corner you will see a cat, that cat is the "mascot" of  gitHub,he is called an Octocat Click on the Octocat and log in with your gitHub
* 3- allow git hub to link the two then create a Cloud9 account. 

### Setting up the link between your GitHub and Cloud9
* 1 - Go to your Github and click on your Icon, Go to the setting, On the Side bar you will see "SSH and GPG keys" Click that and then click "new SSH key"
* 2 - Now go to your Cloud9 and go to the gear icon in the corner on your dashboard, click "SSH Key"
* 3 - Copy the second SSH key you see. 
* 4 - Go back to the SSH key you are making in gitHub and then paste it into the large box. 
* 5 - They click "add SSH key"


---
## Repository Setup

### Remote repository
* 1- Go to github and in the top right there is a "+" icon Click it and then click "new repository"
* 2- Fill in your info and make it public 
* 3- Then add create


### local repository
* 1- Go to cloud9 and on your dashboard click create a new workspace 
* 2- Fill out the Information that pertains to your repo 
        *  repo= repository
* 3- Then create the repo  



---
## Workflow & Commands
### commands 
* **_mkdir_** : creates a directory in your repository
* **_rmdir_** : removes a **empty** directory
* **_git Init_** : initalizes git in your directory, it allows you to use other git commands. **NEVER GIT INIT IN WORKSPACE**
* **_touch Filename.extension_** : creates a file in your directory 
* **_cd directoryName_** : moves you from one directory to another. use when you want to work in a specfic directory.
* **_rm filename_** : removes a specified file 
* **_ rm -rf directoryName_** : allows you to delete filled directories 
* **_ mv_** : use 1: to rename 
* syntax- mv fileNameNow.extension newFileName.extenison 

Use 2: to move a file from one place to another 
* synatx - mv fileName.Extension destination 

* **_git status_** :this shows last edits that were made if they were not commited to the stage they will be in red and if they were commited to the stage then they will be green 
* **_rm -rf .git_** : removes initilized git
* **_git add file.extenison_** :adds a file(S) to the stage that are ready to be committed 
* **_git add_** : adds all files
* **_git add --all_** : adds all files even deleted ones 
* **_git add.txt_** : add all txt files 
* **_git commit -m "message"_** : takes a "snapshot" of the code that you have finished and added to the stage so you have a checkpoint to go to if something  is to break. The -m and the message following it is to allow when you add/commit/push and then you go on github you know what each commit was for by this message. So lets say you changer some markdown and then commit your commit message would say soemthing along the lines of "change markdown". Always make sure the commit messange is in present tense and is USEFUL FOR YOU. creating a good commit message will make it easier to know what screenshot you want to go back to if something again is to break
* **_git remote add origin URL_** : this makes a "rode"/ cnnection to the remote repo or GitHub in this case so ehrn you push it knows where to go 
* **_git push -u origin master_** : pushes your code from the local repository to the remote repository and using -u rembers the place you want to push so you dont have to type "git push origin master" everytime you wanna push so when you would like to push again you can use "git push" adn that will push to the specified repo when you used "git remote add origin URL". 
* **_git pull_** : takes any changes form remote repo and brings them to the local repo 
* **_git diff_** : shows you the differences between your current code and the previous code 
* **_git log_** : shows your previous commits, this will open a new window so when you are done with git log press "Q" to quit git log

### Markdown [help with markdown](https://www.markdowntutorial.com)
* **_Markdown syntax_** : Making a text file look more put together than a large block of text
* _words_ = will italicize by putting underscores before and after the text you want to be italizied 
* **words** = will bold the words you want to be bold by putiing 2 astricks "*" before and after the words 
* **_words_** = will both italicize and bold when you put astiricks and undersocres at the beginning of the phrase/word you want to aplly both too. 
headers= putting a "#" in front of words you can put from 1-6 number signs infront of a phrase. the less amount the larger the heading. 
* links- [name that shows](link) this syntax will create a link to a website 
* list - this makes a list asterisk then a space you can also put a number after the space to create a ordered list. 
* text(space space)= line break 
* `text = one line of code`
* ```texttt = mulitiple lines of text is made with 3 back ticks at the beginning and the end ```

* --- = a line is created with 3 dashes 



---
## Rolling Back Changes

### git checkout -- filename
* disregaurdes edits made in the specified files 
    *if you forget about this command when you use git status after you make a change and you read what it says ou will see this command 


### git reset HEAD filename
* if you add a file to the stage that you didnt want there this will take the specified file away
   *You can find this after you add files to the stage and use git status and read what git staus says you will find this 


### git reset -- soft HEAD 
* undos a commit 
    * look up online how to undo a commit in git and go to stack overflow and you will find it there


### git reset HEAD
* this undos a commit and add to the stage 
    * look up how to undo a commit and add on google and go to stackoverflow 


### git reset -- hard HEAD
* this udos everything, a commit, add , and changes made 
    * look us how to undo add commit anc hanges and go on stack overflow
