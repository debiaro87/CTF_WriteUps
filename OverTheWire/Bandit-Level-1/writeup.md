## OverTheWire bandit: level 0 -level 1

# objective

The main goal of this level is to find the password of level 1 bandit 1 server game that stored in the file called "readme" in home directory.
After finding the password using the password exist in readme file to log in "bandit1" account by using ssh on port 2220.

# to solve this I pass through four steps . let's see one by one 

## step_1: connect to bandit0 server

connect to bandit0 server by using ssh command on port 2220 and given password for me . that is:
        " ssh bandit0@bandit.labs.overthewire.org -p 2220 "
After entering the password I successfully logged in bandit0

## step_2: check the files

To check the file exist in the current directory I use the command "ls".

bash:
ls

Since I am in home directory i got "readme" file 

## step_3: read the file
To read the text or content exist in "readme" file I use the command "cat" 

bash:
cat readme
ow that's great I got what i want that is the password of bandit1 
## Step_4:Log in to bandit 1
To log in bandit1 I use ssh command on port 2220 and password i get from bandit0 readme file 
The first command I use is:

bash:
ssh bandit1@bandit.labs.overthewire.org -p 2220

Then it asked me to enter the password for authenticity since i have got a password from readme file i enter the password and finally I successfully logged in as bandit1 server user.

# what i learned from this bandit1 level:
          Using SSH to connect to remote server 
          
