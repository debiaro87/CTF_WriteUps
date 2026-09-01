## Bandit Level 1 → Level 2

# OBJECTIVE
The main goal of this level is to find the password of bandit level 2 in the "-" file that exist in  home directory. 

After finding the password , use it to log in to "bandit_2" account by using ssh on port "2220"
## To solve this we pass through three steps:
## step 1: logging in to bandit_1:

First we have to log in as bandit_1 in to the server, to do that we write a command :

bash:

SSH bandit1@bandit.labs.overthewire.org -p 2220

After that it ask as the password to authenticity, since we have a password we get in level 1 from a file "-" we enter that password then we successfully  logged in as bandit_2 

