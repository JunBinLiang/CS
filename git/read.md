
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
 - **git commit --amend** : Redo the previous commit

 <br/>
 
### Git-Ignore

 - **.DS_Store** : ignore file named ".DS_Store"
 - **folder/** : ignore folder
 - ****.log*** : ignore all file with extension .log


<br/><br/>
## 2. Git Branching

### Create/Switch
 - **git branch** : view all available branches
 -   **git branch name** : creates a branch
-   **git switch name** : switch a branch (Be careful with Switching with nnstaged change)

 <br/>

### Rename/Delete

 - **git branch -D name** : delete the branch (force delete by using Capital D)
 - **git branch -m newname** : rename
 
<br/><br/>
## 3. Merging

### 1. Merging Flow

>Flow : 
>git switch branch-> git merge branch

<br/><br/>

>With Conflicts : 
>git switch branch-> git merge branch -> resolve conflicts -> git add -> git commit

<br/><br/>
## 3. Git Diff

### Git Diff
 - **git diff** : without additional option, it lists all the changes in our working directory that are not staged for the next commit. 
 - **git diff HEAD** : lists all changes since last commit
- **git diff stage** : lists all changes that are staged
- **git diff option filename** : list change for a single file
- **git diff branch1..branch2** : diff for 2 different branches



<br/><br/>
## 3. Stash
**Situation** : When you make some change on current branch, you did not commit and you want to switch to other branch. <br/>
**1**. Not allow if there is conflicts. <br/>
**2**. Bring those change to the branch you switch<br/>

<br/>

**Stash** : Save the change without commit and get them back later

<br/><br/>
### Git Stash

 - **git stash** : save the uncommit changes
 - **git pop** : retrieve those changes from the stash
 - **git apply** : apply the change instead of pop, contents are still on the stash
	
