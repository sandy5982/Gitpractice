---
title: "Github commands for begginer"
author: "Sandeep First Tutorial"
date: "May 10, 2017"
output: html_document
---

`# First step is to open R markdown and save it in a file or desktop
## knit to HTML
## make a directory in desktop

cd Desktop    
## to enter in desktop

mkdir GitHub  
## creating a directory on desktop

mv * GitHub 
## mv command is used to move files
## Github is moved from desktop in a previously created directory GitHub
## * is used to move all files with name Github (more files with same name)

cd GitHub  ## to enter in GitHub directory

## Enter in R to change RMD to md
## Github does not take RMD file 

R

knitr::knit (input = "Github.Rmd, output = "README.md")
## now README.md file will be ready

q() ## quit R


## now initializing GitHub

git init
## Initialized empty Git repository in /home/sandeepsingh/Desktop/GitHub/.git/

## create a new repositry in Github (Gitpractice)

## adding Github file in repository

git remote add origin https://github.com/sandy5982/Gitpractice.git

## if origin is not available it will show mistake then

git remote add myorigin https://github.com/sandy5982/Gitpractice.git

## OR

git remote add testtest https://github.com/sandy5982/Gitpractice.git

git remote -v
## origin	https://github.com/sandy5982/Gitpractice.git (fetch)
## origin	https://github.com/sandy5982/Gitpractice.git (push)

git add README.md

git status

git commit -m "Added README" README.md
 
git push origin master
 ## it will ask for ID pw for github online
 
 ## now adding R Scripts in local and push it into github
 ## most of these commands are similar
 ## Make an R script first and save it by a name in GitHub directory
 
git add Script.R
 
git commit -m "Added Script" Script.R

git push origin master
## it will ask for GitHub ID and Password

## We can do changes in R script in R studio and then save it again in Github

git add Script.R

git commit -m "chnages" Script.R

git push origin master  ## again ID and PW


 
 




