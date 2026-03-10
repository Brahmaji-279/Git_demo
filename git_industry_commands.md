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

<img width="1103" height="385" alt="Screenshot from 2026-03-10 14-59-43" src="https://github.com/user-attachments/assets/98606fa2-fb6d-44ed-b0a0-a7107ab2d2fb" />
# Repository setup commands
(i) git init
  ->Used to initialize a git repository in a local folder
  ->Syntax: git init
(ii) git clone
   ->Used to clone a existing repository in the local folder
   ->Syntax:git clone "repo url"
(iii)git 
