# Git
### What is Git ?

 - Version Control System <br/>
 - Track and manage changes <br/>
 - Collaboration, Combining/Sharing Changes<br/>

### What is GitHub ?

 - Web Service<br/>
 - Hosting Git Project in cloud for easy Colloboration<br/>


<br/><br/>
## 1. Git Basic
**Git WorkFlow**
>Working On Stuff -> Add Change -> Commit<br/><br/>

<br/>

### Create 
 - **git status** : Information of the repository<br/>
 - **git init** : instantiates a new repository ( **Warn** : Don't nested Git repository)<br/>
 <br/>

### Commit

 - **git add name.txt** : staging the changes
 - **git commit -m "my message"** : commit, includes message to summarize the changes
 - **git log** : view the commit history
 <br/>

### Amending
 **git commit --amend** : Redo the previous commit

 <br/>
 
### Git-Ignore

 - **.DS_Store** : ignore file named ".DS_Store"
 - **folder/** : ignore folder
 - *.log : ignore all file with extension .log


<br/><br/>
## 2. Git Branching

### Create/Switch
 - **git branch** : view all available branches
 -   **git branch name** : creates a branch
-   **git switch name** : switch a branch (Be careful with Switching with nnstaged change)

 <br/>
