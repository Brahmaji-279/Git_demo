# Git Configuration Commands

## 1. Git Configuration Commands

### (i) `git config --global user.name`

- Used to configure the **username of our GitHub account** in the local machine.

- **Example**

```bash
git config --global user.name Brahmaji-220671
```

---

### (ii) `git config --global user.email`

- Used to configure the **email of the GitHub account** used in the local machine.

- **Example**

```bash
git config --global user.email n220671@rguktn.ac.in
```

---

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

---

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
---
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

---

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

---

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

---

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

---

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
---
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

---

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
---
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
---
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
---
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
---
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
---
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
---
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

---

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

---

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

---

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

---

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

---

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

---

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

---

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

<img width="1366" height="768" alt="Screenshot from 2026-03-28 20-36-31" src="https://github.com/user-attachments/assets/47b6d272-5826-475e-824d-0d5ebff77b19" />

