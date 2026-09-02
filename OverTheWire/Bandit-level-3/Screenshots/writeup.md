## Bnadit Level 2-3

# OBJECTIVE
The main goal of this level is to find the password of bandit level 3 in the "--spaces in this filename--" file that exist in  home directory. 

After finding the password , use it to log in to "bandit_3" account by using ssh on port "2220"
## To solve this we pass through three steps:
## step 1: logging in to bandit_2:

First we have to log in as bandit_2 in to the server, to do that we write a command :

bash:

SSH bandit2@bandit.labs.overthewire.org -p 2220

After that it ask as the password to authenticity, since we have a password we get in level 1 from a file "-" we enter that password then we successfully  logged in as bandit_2 

