## :rocket: Tech Stacks
- Full fledged guide for initialising and firing up development tools such as database management systems, development frameworks, packages and version managers
<br>


## MacOS Unix Shell: zsh 
- Default shell for macOS (earlier versions use bash instead of zsh)
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
$ git commmit -m "insert commit message" to create a new commit with your staged changes

# Push changes
$ git push {remote repository name} {branch name} 
$ git push origin main # for pushing into main branch
```
<br>


## Languages and frameworks

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


## Packages installed

#### nvm (node version manager)
- version manager for nodejs
- [link to install packages](https://github.com/nvm-sh/nvm)
- [tutorial on installation](https://www.youtube.com/watch?v=ohBFbA0O6hs)

#### nodemon
- tool that automatically restarts node applications when file changes in the directory are detected
- [link to nodemon site](https://www.npmjs.com/package/nodemon`)
- `npm install -g nodemon` to install
- `nodemon {insert file name in current directory}` eg. `nodemon app` to use tool
<br>


## NodeJS
- Backend server runtime environment for running javascript 

#### Helpful tutorials
- [creating a node app](https://www.youtube.com/watch?v=EMwu8F0dCXE&t=1452s)
<br>


## Directories and files

#### libraries installed
- express `npm install express --save`
- path `npm install path --save`
- ejs `npm install ejs --save`
<br>


## MySQL
- [Installation and Setup](https://www.youtube.com/watch?v=oxToe-4c6OM)

Installation & Setup (for zsh shell)
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



