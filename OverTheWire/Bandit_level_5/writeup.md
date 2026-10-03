# Bandit Level 4 → Level 5

## OBJECTIVE 
The main goal of this level is to find the password of bandit level 5 that exist in human read able file in "inhere" directory

## 1 connect to bandit 4:
To connect to bandit 4 we write a command :

bash:

ssh bandit4@bandit.labs.overthewire.org -p 2220

Output:
<img width="1280" height="800" alt="Command4" src="https://github.com/user-attachments/assets/b3f9f80e-c7aa-44ec-8512-a15307a802a5" />


## 2 check a file :

To check whether a file exist or not we write a command :

bash:

ls

we get "inhere" directory not file

## 3 Change directory :

To change the directory 

bash:

cd inhere

now we are in the inhere directory 
## 4 check a file :

To check whether a file exist in inhere directory or not we write a command 

ls

then we get the list of files as we see on the screenshot below
<img width="1280" height="800" alt="list,change,list" src="https://github.com/user-attachments/assets/3de038fe-2b1d-4b86-bcdc-ab247b5b3025" />
## 5 identify the type of file :
since there is so many file in the inhere directory we should have to identify the type of each file we use a command 

bash

file./*

from those i looked for the file identified as human-readable/ASCII TEXT as we see from screenshot below 
<img width="1280" height="800" alt="type of file" src="https://github.com/user-attachments/assets/c18825d7-8ee6-4d17-b7d8-66d955164594" />


## 6 read a file :
To read the content of the human-readable/ASCII text file we use a command 

bash

cat ./-file07


finally we get the password of bandit level 5 
<img width="1280" height="800" alt="Done" src="https://github.com/user-attachments/assets/91039838-cdc5-4b31-b298-aa425376f434" />

## What i learned :
              ls ~ list files 
              file ./* ~ identify the type of all files
              cat ./-filename ~ read a file 
## Platform





