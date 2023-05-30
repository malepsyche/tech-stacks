## :rocket: Tech Stacks
- Full fledged guide for initialising and firing up development tools such as full-stack frameworks, version managers, packages and database management systems.
- Note: This guide is mainly specialised for Apple Silicon Mac users with zsh unix shell as opposed to bash. Some parts of this guide may not be 100% applicable to those who do not meet this criteria.
<br>


## MacOS Unix Shell: zsh 
- Default shell for macOS (earlier versions use bash instead of zsh)
<br>


## Git
- Version control system that records changes to file(s) over time so that you can recall specific versions later
- [Installation & Configuration](https://www.theodinproject.com/lessons/foundations-setting-up-git)

```zsh
# File Permissions Guide
nanika@vultr:~/code-server/vscode/CRM_motosing$ ls -l
total 16
drwxr-xr-x 7 root root 4096 May 26 13:49 new-crm-project
drwxr-xr-x 6 root root 4096 May 18 08:39 old-crm-project-v1
drwxr-xr-x 7 root root 4096 May 12 12:53 old-crm-project-v2
-rw-r--r-- 1 root root   91 May 12 12:53 package-lock.json
# In the output of the `ls -l` command, file permissions are represented by a 10-character string. Let's break down the structure:
drwxr-xr-x
# The first character indicates the type of the file. If it is a directory, it will be `d`. For regular files, it will be `-`.
# The next three characters represent the permissions of the owner (user) of the file/directory. These characters can be `r` for read, `w` for write, or `x` for execute permissions.
# The following three characters represent the permissions of the group that the file/directory belongs to.
# The final three characters represent the permissions for others (users not in the owner group).
r, w, x & -
# Each character in the file permission string represents a specific permission type. Here are the possible permission types:
r # read: Allows the user to read the file's content or list the directory's contents.
w # write: Allows the user to modify the file or directory, including creating, deleting, or renaming files within a directory.
x # execute: Allows the user to execute a file or access a directory's contents and navigate through it.
- # If a permission is not granted, a `-` is used in its place.
# Each set of three characters in the file permission string represents permission assignments for different entities:
# Owner (user): The user who owns the file or directory.
# Group: A group of users to which the file or directory belongs.
# Others: Users who are not the owner or part of the group.
drwxr-xr-x
# The first character `d` indicates that it is a directory.
# The next three characters, `rwx`, represent the permissions of the owner. In this case, the owner has read, write, and execute permissions.
# The next three characters, `r-x`, represent the permissions of the group. The group has read and execute permissions.
# The final three characters, `r-x`, represent the permissions for others. Others have read and execute permissions.


# User Identification Guide
nanika@vultr:~/code-server/vscode/CRM_motosing$ id
uid=1001(nanika) gid=1001(nanika) groups=1001(nanika),27(sudo)
uid # Your user ID, which uniquely identifies your user account.
gid # Your group ID, which identifies the primary group associated with your user account.
groups # Additional groups you belong to, if any.
# If your `uid` matches the `gid` value, you are the owner of the file or directory.
# If your `uid` matches one of the `groups`, you belong to the group associated with that ID.
# If your `uid` doesn't match the `gid` or any of the `groups`, you fall under the "others" category.
```
<br>



## Github
```zsh
# Code repository platform for development

# Clone repository
$ git clone {repository_url} {destination_folder} # to clone online repository into local file  
$ git clone https://github.com/malepsyche/tech-stacks ~/Documents/tech-stack

# File checks 
$ git status # to see which files are modified and which files are staged or unstaged: 
$ git diff # to see the detailed line-by-line differences of the changes in each file: 

# Stage file changes
$ git add {file name} # to stage individual file changes
$ git add . # to stage all file changes

# Commit changes
$ git commmit -m "insert commit message" # to create a new commit with your staged changes

# Push changes
$ git push {remote repository name} {branch name} 
$ git push origin main # for pushing into main branch

# Merge branches 
$ git fetch
$ git log --graph --oneline {remote repository name} {branch name}
$ git merge {remote repository name} {branch name} 

# Rebase branches 
$ git fetch
$ git log --graph --oneline {remote repository name} {branch name}
$ git rebase {remote repository name} {branch name} 

# Fetch and overwrite local
$ git fetch origin
$ git reset --hard origin/<branch-name>
```
<br> 


## Languages & Frameworks 

#### Frontend
- ejs
- react
- css: bootstrap

#### Backend & API
- nodejs
- express

#### Database
- postgreSQL
- MySQL
<br>


## NodeJS
- Backend server runtime environment for running javascript 
- [How to create a Node Application](https://www.youtube.com/watch?v=EMwu8F0dCXE&t=1452s)

#### Step 1: Install Packages

#### nvm (node version manager)
- Version manager for nodejs
- [Link to install packages](https://github.com/nvm-sh/nvm)
- [Tutorial on installation](https://www.youtube.com/watch?v=ohBFbA0O6hs)

#### nodemon
- Tool that automatically restarts node applications when file changes in the directory are detected
- [Link to nodemon site](https://www.npmjs.com/package/nodemon`)
- `npm install -g nodemon` to install
- `nodemon {insert file name in current directory}` eg. `nodemon app` to use tool
<br>

#### Step 2: Install Libraries

#### Fundamental libraries
- express (api) `npm install --save express `
- path (module for working with directory paths) `npm install --save path `

#### Client-side scripting
- ejs (embedded javascript) `npm install ejs --save`

#### Middleware
- [multer middleware](https://github.com/expressjs/multer) (used for uploading files) `npm install --save multer`
<br>


## MySQL

#### Install MySQL 
- [Installation and Setup](https://www.youtube.com/watch?v=oxToe-4c6OM)

#### Setup (for zsh shell)
```zsh
$ cd ~ # Go to home directory
$ nano .zprofile # open .zprofile file 

# Set PATH for MySQL 8.0.33
$ export PATH=${PATH}:/usr/local/{insert path name of bin folder}
$ export PATH=${PATH}:/usr/local/mysql-8.0.33-macos13-arm64/bin

# Connect to MySQL
$ mysql -u root -p
```
<br>



