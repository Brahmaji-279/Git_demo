# Git Configuration Commands
## 1. Git Configuration Commands
### (i) `git config --global user.name`
- Used to configure the **username of our GitHub account** in the local machine.
- **Example**
```bash
git config --global user.name Brahmaji-220671
```
### (ii) `git config --global user.email`
- Used to configure the **email of the GitHub account** used in the local machine.
- **Example**
```bash
git config --global user.email n220671@rguktn.ac.in
```
### (iii) `git config --list`
- Used to **list all available configuration variables and settings** in the local machine.
- **Example**
```bash
git config --list
```
Example Output:
```bash
user.email=n220671@rguktn.ac.in
user.name=Brahmaji-220671
credential.helper=store
pull.rebase=false
log.abbrevcommit=true
safe.directory=/opt/lampp/htdocs/php_CyberAwarenessWebsite
safe.directory=/opt/lampp/htdocs/php_CyberAwarenessWebsite/CybersecurityAwarenessWebsite
http.postbuffer=524288000
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
remote.origin.url=https://github.com/Brahmaji-279/WT_LAB.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
```
### (iv) `git config --unset`
- Used to **remove a specific configuration line** from the configuration file.
- **Syntax**
```bash
git config [--local | --global | --system] --unset <key>
```
- **Example**
To remove the username:
```bash
git config --global --unset user.name
```
- **Screenshot**
![Git Demo Screenshot](https://github.com/user-attachments/assets/98606fa2-fb6d-44ed-b0a0-a7107ab2d2fb)
## Repository Setup Commands
## 1. git init
**Purpose:**  
Initializes a new Git repository in a local folder.
### Syntax
```bash
git init
```
### Example
```bash
git init
```
## 2. git clone
**Purpose:**  
Clones an existing repository into the local system.
### Syntax
```bash
git clone <repository_url>
```
### Example
```bash
git clone https://github.com/Brahmaji-279/Git_demo.git
```
## 3. git clone --branch
**Purpose:**  
Clones a specific branch instead of the default branch.
### Syntax
```bash
git clone --branch <branch_name> <repository_url>
```
### Example
```bash
git clone --branch first_branch https://github.com/Brahmaji-279/Git_demo.git
```
## 4. git clone --depth
**Purpose:**  
Creates a shallow clone with limited repository history. Useful when the repository is large.
### Syntax
```bash
git clone --depth <number> <repository_url>
```
### Example
```bash
git clone --depth 1 https://github.com/Brahmaji-279/Git_demo.git
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/16e9ab36-6c44-4ca7-9492-84008786e927)
#Repository Status & Inspection
## 1. git status
**Purpose:**
Used to check the status of the git repository we created.
### Syntax
```bash
git status
```
### Example
```bash
git status
```
## 2. git log
**Purpose:**
To check the history of commited changes within a git repository.
### Syntax
```bash
git log
```
### Example
```bash
git log
```
## 3. git log --oneline
**Purpose:**
Used to display the commit history in a compact format
### Syntax
```bash
git log --oneline
```
### Example
```bash
git log -oneline
```
## 4. git log --graph
**Purpose:**
Used to visualize the branching and merging structure of the repostitory.
### Syntax
```bash
git log --graph
```
### Example
```bash
git log --graph
```
## 5.git show
**Purpose:**
 Used to shows the fil of the repository
 ### Syntax
 ```bash
git show
```
### Example 
```bash
git show
```
## 6.git diff 
**Purpose:**
used to display the differences between two versions of files within a repository
### Syntax
```bash
git diff
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/6e4e646f-6a2e-473a-bf21-9c79f6a8117d)
## git diff --staged
**Purpose:**  
Shows the differences between the staged files and the last commit.
### Syntax
```bash
git diff --staged
```
### Example
```bash
git add file1.txt
git diff --staged
```
## git blame
**Purpose:**  
Displays who last modified each line of a file along with the commit information.
### Syntax
```bash
git blame <file_name>
```
### Example
```bash
git blame index.html
```
## git reflog
**Purpose:**  
Shows a log of all recent actions performed in the repository such as commits, resets, and checkouts.
### Syntax
```bash
git reflog
```
### Example
```bash
git reflog
```
## git shortlog
**Purpose:**  
Summarizes commit history grouped by author.
### Syntax
```bash
git shortlog
```
### Example
```bash
git shortlog
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/ad86720a-a036-466e-9409-be236125aa4c)
# File Tracking Commands
## git add
**Purpose:**  
Adds specific files to the staging area before committing.
### Syntax
```bash
git add <file_name>
```
### Example
```bash
git add index.html
```
## git add .
**Purpose:**  
Adds all modified and new files in the current directory to the staging area.
### Syntax
```bash
git add .
```
### Example
```bash
git add .
```
## git add -p
**Purpose:**  
Allows you to stage changes interactively by selecting specific parts of a file.
### Syntax
```bash
git add -p
```
### Example
```bash
git add -p app.js
```
## git restore
**Purpose:**  
Restores a file in the working directory to the last committed state.
### Syntax
```bash
git restore <file_name>
```
### Example
```bash
git restore index.html
```
## git restore --staged
**Purpose:**  
Removes a file from the staging area but keeps the changes in the working directory.
### Syntax
```bash
git restore --staged <file_name>
```
### Example
```bash
git restore --staged app.js
```
## git rm
**Purpose:**  
Removes a file from both the working directory and the Git repository.
### Syntax
```bash
git rm <file_name>
```
### Example
```bash
git rm old_file.txt
```
## git mv
**Purpose:**  
Moves or renames a file and stages the change automatically.
### Syntax
```bash
git mv <old_name> <new_name>
```
### Example
```bash
git mv old_name.txt new_name.txt
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/a8bb5de5-be43-448c-b6bc-75bfab381585)
# Commit commands
## git commit 
**Purpose:**
Commits a specific message for the changes it opens a window to enter the commit
### Syntax 
```bash
git commit 
```
### Example 
```bash
git commit
```
## git commit -m 
**Purpose:**
Enters the commit message within the command
### Syntax
```bash
git commit -m <text as commit>
```
### Example 
```bash
git commit -m "Some files are added"
```
## git commit --amend
**Purspose:**
Reviews the last commit using a window to edit last commit
### Syntax 
```bash
git commit --amend
```
### Example 
```bash
git commit --amend
```
## git commit --no-edit
**Purpose:**
Used to add more files without changing the before commit 
## Syntax
```bash
git commit --no-edit
```
## Example
```bash
git add .
git commit --no-edit
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/5ad7de52-928f-468a-a4e0-df71a18fc3bb)
# Branch Management Commands
## git branch  
**Purpose:**  
Lists all local branches in the repository  
### Syntax  
```bash
git branch
```
### Example  
```bash
git branch
```
## git branch -a  
**Purpose:**  
Lists all branches (local + remote)  
### Syntax  
```bash
git branch -a
```
### Example  
```bash
git branch -a
```
## git branch -d  
**Purpose:**  
Deletes a branch safely (only if it is already merged)  
### Syntax  
```bash
git branch -d <branch-name>
```
### Example  
```bash
git branch -d first_branch
```
## git branch -D  
**Purpose:**  
Force deletes a branch (even if it is not merged)  
### Syntax  
```bash
git branch -D <branch-name>
```
### Example  
```bash
git branch -D new_branch
```
## git checkout  
**Purpose:**  
Switches to an existing branch  
### Syntax  
```bash
git checkout <branch-name
```
### Example  
```bash
git checkout new2
```
## git checkout -b  
**Purpose:**  
Creates a new branch and switches to it immediately  
### Syntax  
```bash
git checkout -b <branch-name>
```
### Example  
```bash
git checkout -b new3
```
## git switch  
**Purpose:**  
Switches between branches (modern replacement for checkout)  
### Syntax  
```bash
git switch <branch-name>
```
### Example  
```bash
git switch main
```
## git switch -c  
**Purpose:**  
Creates a new branch and switches to it (modern alternative to checkout -b)  
### Syntax  
```bash
git switch -c <branch-name>
```
### Example  
```bash
git switch -c new4
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/47b6d272-5826-475e-824d-0d5ebff77b19)
#  Merge & Integration Commands
## git merge  
**Purpose:**  
Combines changes from one branch into the current branch  
### Syntax  
```bash
git merge <branch-name>
```
### Example  
```bash
git checkout main
git merge new4
```
## git merge --no-ff  
**Purpose:**  
Merges a branch while preserving a separate merge commit (no fast-forward)  
### Syntax  
```bash
git merge --no-ff <branch-name>
```
### Example  
```bash
git checkout main
git merge --no-ff new4
```
## screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/12fe4245-e259-4918-a971-240cb481ee25)
# Remote Repository Commands
## git remote  
**Purpose:**  
Shows the list of remote repositories linked to your project  
### Syntax  
```bash
git remote
```
### Example  
```bash
git remote
```
## git remote -v  
**Purpose:**  
Displays remote repositories with their URLs  
### Syntax  
```bash
git remote -v
```
### Example  
```bash
git remote -v
```
## git remote add  
**Purpose:**  
Adds a new remote repository  
### Syntax  
```bash
git remote add <name> <url>
```
### Example  
```bash
git remote add origin https://github.com/user/repo.git
```
## git remote remove  
**Purpose:**  
Removes an existing remote repository  
### Syntax  
```bash
git remote remove <name>
```
### Example  
```bash
git remote remove origin
```
## git fetch  
**Purpose:**  
Downloads changes from the remote without merging  
### Syntax  
```bash
git fetch
```
### Example 
```bash
git fetch
```
## git fetch --all  
**Purpose:**  
Fetches updates from all remotes  
### Syntax  
```bash
git fetch --all
```
### Example  
```bash
git fetch --all
```
## git pull  
**Purpose:**  
Fetches and merges changes from the remote repository  
### Syntax  
```bash
git pull <remote> <branch>
```
### Example  
```bash
git pull origin main
```
## git pull --rebase  
**Purpose:**  
Fetches changes and rebases your commits on top of them  
### Syntax  
```bash
git pull --rebase <remote> <branch>
```
### Example  
```bash
git pull --rebase origin main
```
## git push  
**Purpose:**  
Uploads local commits to the remote repository  
### Syntax  
```bash
git push <remote> <branch>
```
### Example  
```bash
git push origin main
```
## git push -u origin <branch-name>  
**Purpose:**  
Pushes the branch and sets upstream tracking  
### Syntax  
```bash
git push -u origin <branch-name>
```
### Example  
```bash
git push -u origin feature-login
```
## git push --force  
**Purpose:**  
Force pushes changes (overwrites remote history)  
### Syntax  
```bash
git push --force
```
### Example  
```bash
git push --force
```
## Screenshot 
![Git Demo Screenshot](https://github.com/user-attachments/assets/9473e821-a29f-4d4c-b15a-d2cf90278474)
# Stash Commands
## git stash  
**Purpose:**  
Temporarily saves uncommitted changes and cleans the working directory  
### Syntax  
```bash
git stash
```
### Example  
```bash
git stash
```
## git stash list  
**Purpose:**  
Shows all stashed changes  
### Syntax  
```bash
git stash list
```
### Example  
```bash
git stash list
```
## git stash pop  
**Purpose:**  
Applies the latest stash and removes it from the stash list  
### Syntax  
```bash
git stash pop
```
### Example  
```bash
git stash pop
```
## git stash apply  
**Purpose:**  
Applies a stash without removing it from the list  
### Syntax  
```bash
git stash apply
```
### Example  
```bash
git stash apply
```
## git stash drop  
**Purpose:**  
Deletes a specific stash  
### Syntax  
```bash
git stash drop <stash-id>
```
### Example  
```bash
git stash drop stash@{0}
```
## git stash clear  
**Purpose:**  
Deletes all stashes permanently  
### Syntax  
```bash
git stash clear
```
### Example  
```bash
git stash clear
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/5a48b497-f4bc-490a-a30a-eda2f670f054)
# Reset & Undo Commands
## git reset  
**Purpose:**  
Resets the current HEAD to a specified state  
### Syntax  
```bash
git reset <commit>
```
### Example  
```bash
git reset HEAD~1
```
## git reset --soft  
**Purpose:**  
Moves HEAD to a previous commit but keeps changes staged  
### Syntax  
```bash
git reset --soft <commit>
```
### Example  
```bash
git reset --soft HEAD~1
```
## git reset --mixed  
**Purpose:**  
Moves HEAD to a previous commit and unstages changes (default reset)  
### Syntax  
```bash
git reset --mixed <commit>
```
### Example  
```bash
git reset --mixed HEAD~1
```
## git reset --hard  
**Purpose:**  
Moves HEAD to a previous commit and deletes all changes permanently  
### Syntax  
```bash
git reset --hard <commit>
```
### Example  
```bash
git reset --hard HEAD~1
```
## git revert  
**Purpose:**  
Creates a new commit that undoes changes from a previous commit  
### Syntax  
```bash
git revert <commit>
```
### Example  
```bash
git revert HEAD
```
## git clean -f  
**Purpose:**  
Removes untracked files from the working directory  
### Syntax  
```bash
git clean -f
```
### Example  
```bash
git clean -f
```
## git clean -fd  
**Purpose:**  
Removes untracked files and directories  
### Syntax  
```bash
git clean -fd
```
### Example  
```bash
git clean -fd
```
# Rebasing Commands
## git rebase  
**Purpose:**  
Reapplies commits from one branch onto another base branch  
### Syntax  
```bash
git rebase <branch-name>
```
### Example  
```bash
git checkout new4
git rebase main
```
## git rebase -i  
**Purpose:**  
Interactive rebase to edit, squash, reorder, or delete commits  
### Syntax  
```bash
git rebase -i <commit>
```
### Example  
```bash
git rebase -i HEAD~3
```
## git rebase --continue  
**Purpose:**  
Continues the rebase process after resolving conflicts  
### Syntax  
```bash
git rebase --continue
```
### Example  
```bash
git rebase --continue
```
## git rebase --abort  
**Purpose:**  
Cancels the rebase and restores the previous state  
### Syntax  
```bash
git rebase --abort
```
### Example  
```bash
git rebase --abort
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/b895f1ad-9b17-46c0-842d-5750ac6db797)
# Cherry Pick & Patch Commands
## git cherry-pick  
**Purpose:**  
Applies a specific commit from one branch to another  
### Syntax  
```bash
git cherry-pick <commit-hash>
```
### Example  
```bash
git checkout main
git cherry-pick a1b2c3d
```
## git format-patch  
**Purpose:**  
Creates patch files from commits for sharing changes  
### Syntax  
```bash
git format-patch <commit>
```
### Example  
```bash
git format-patch HEAD~2
```
## git apply  
**Purpose:**  
Applies a patch file to the working directory (no commit created)  
### Syntax  
```bash
git apply <patch-file>
```
### Example  
```bash
git apply 0001-fix-login.patch
```
## git am  
**Purpose:**  
Applies patch files and creates commits from them  
### Syntax  
```bash
git am <patch-file>
```
### Example  
```bash
git am 0001-fix-login.patch
```
# Tagging Commands
## git tag  
**Purpose:**  
Lists all tags in the repository  
### Syntax  
```bash
git tag
```
### Example  
```bash
git tag
```
## git tag -a  
**Purpose:**  
Creates an annotated tag with a message  
### Syntax  
```bash
git tag -a <tag-name> -m "message"
```
### Example  
```bash
git tag -a v1.0 -m "Initial release"
```
## git tag -d  
**Purpose:**  
Deletes a tag locally  
### Syntax  
```bash
git tag -d <tag-name>
```
### Example  
```bash
git tag -d v1.0
```
## git push origin --tags  
**Purpose:**  
Pushes all local tags to the remote repository  
### Syntax  
```bash
git push origin --tags
```
### Example  
```bash
git push origin --tags
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/b315fcfa-aaeb-45df-bd83-525eca587c06)
# Submodule Commands
## git submodule add  
**Purpose:**  
Adds another Git repository as a submodule inside your project  
### Syntax  
```bash
git submodule add <repository-url>
```
### Example  
```bash
git submodule add https://github.com/user/library.git
```
## git submodule init  
**Purpose:**  
Initializes submodules (sets up configuration locally)  
### Syntax  
```bash
git submodule init
```
### Example  
```bash
git submodule init
```
## git submodule update  
**Purpose:**  
Fetches and checks out the correct version of submodules  
### Syntax  
```bash
git submodule update
```
### Example  
```bash
git submodule update
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/b0da09af-35aa-4ba5-bb8b-7c7e04adfb26)
# Debugging Commands
## git bisect  
**Purpose:**  
Helps find the commit that introduced a bug using binary search  
### Syntax  
```bash
git bisect
```
### Example  
```bash
git bisect
```
## git bisect start  
**Purpose:**  
Starts the bisect process  
### Syntax  
```bash
git bisect start
```
### Example  
```bash
git bisect start
```
## git bisect good  
**Purpose:**  
Marks a commit as good (no bug present)  
### Syntax  
```bash
git bisect good <commit>
```
### Example  
```bash
git bisect good a1b2c3d
```
## git bisect bad  
**Purpose:**  
Marks a commit as bad (bug present)  
### Syntax  
```bash
git bisect bad <commit>
```
### Example  
```bash
git bisect bad HEAD
```
## Screenshot
![Git Demo Screenshot](https://github.com/user-attachments/assets/04760693-364c-462f-8615-5dec22d9bf67)
