## :rocket: Tech Stacks
- Full fledged guide for initialising and firing up development tools such as full-stack frameworks, version managers, packages and database management systems.
- Note: This guide is mainly specialised for Apple Silicon Mac users with zsh unix shell as opposed to bash. Some parts of this guide may not be 100% applicable to those who do not meet this criteria.
<br>


## MacOS Unix Shell: zsh 
- Default shell for macOS (earlier versions use bash instead of zsh)
<br>


## Git
- Version control system that tracks changes in any set of computer files
- [Installation & Configuration](https://www.theodinproject.com/lessons/foundations-setting-up-git)
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



