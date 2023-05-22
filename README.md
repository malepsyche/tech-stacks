# Tech Stacks
- Full fledged guide for initialising and firing up tools such as database management systems, development frameworks, packages and version managers

## MacOS Unix CLI: Bash

## Github
- Code repository platform for development

### Clone repository
- Clone online repository into local file: `git clone {repository_url} {destination_folder}` eg. `git clone https://github.com/malepsyche/tech-stacks ~/Documents/tech-stack` 

### File checks
- See which files are modified and which files are staged or unstaged: `git status`
- See the detailed line-by-line differences of the changes in each file: `git diff`

### Stage file changes
- `git add {file name}` to stage individual file changes
- `git add .` to stage all file changes

### Commit changes
- `git commmit -m "insert commit message"` to create a new commit with your staged changes

### Push changes
- `git push {remote repository name} {branch name}` eg. `git push origin main` for pushing into main branch


## Languages and frameworks

frontend
- ejs
- react
- css: bootstrap

backend
- nodejs
- express

database
- postgreSQL
- MySQL


## Packages installed

### nvm (node version manager)
- version manager for nodejs
- [link to install packages](https://github.com/nvm-sh/nvm)
- [tutorial on installation](https://www.youtube.com/watch?v=ohBFbA0O6hs)

### nodemon
- tool that automatically restarts node applications when file changes in the directory are detected
- [link to nodemon site](https://www.npmjs.com/package/nodemon`)
- `npm install -g nodemon` to install
- `nodemon {insert file name in current directory}` eg. `nodemon app` to use tool
______________________________________________________
<br/>

# Introduction

## Helpful tutorials
- [creating a node app](https://www.youtube.com/watch?v=EMwu8F0dCXE&t=1452s)

______________________________________________________
<br/>

# Directories and files

## app.js
- main application file
- `./app.js`

## views dir
- directory that stores ejs files (html with embedded javascript)
- `./views`

## css dir
- bootstrap code
- `./css`

## routes dir
- directory that stores javascript files for each individual view page routing
- `./routes`

## libraries installed
- express `npm install express --save`
- path `npm install path --save`
- ejs `npm install ejs --save`

______________________________________________________





