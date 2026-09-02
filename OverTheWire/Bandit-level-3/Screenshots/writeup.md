## Bandit Level 2 → Level 3

# OBJECTIVE
The main goal of this level is to find the password of bandit level 3 in the "--spaces in this filename--" file that exist in  home directory of bandit level 2. 

After finding the password , use it to log in to "bandit_3" account by using ssh on port "2220"
## To solve this we pass through three steps:
## step 1: log in to Bandit_2

First we have to log in as bandit_2 in to the server, to do that we write a command :

bash:

SSH bandit2@bandit.labs.overthewire.org -p 2220

After that it ask us the password to authenticity, since we have a password we get in level 1 from a file "-" we enter that password then we successfully  logged in as bandit_2 

The output of the command:

<img width="1920" height="1080" alt="COMMAND-2" src="https://github.com/user-attachments/assets/4cdfa3fc-403f-4065-98d6-9aad330f3b8b" />


## Step 2: check the file

To check the file whether it exist or not  we use a command:

bash:


ls

## Step 3: Read the file

Since the file exist to read the content of the file we use a command:

bash:

cat --"--spaces in this filename--"

right we get the password of bandit level 3 . we have to copy the password and exit the server 

## Step 4: log in to Bandit 3

To log in as bandit 3 server first we have log out the previous bandit server  and we write a command :

bash:

ssh bandit3@bandit.labs.org -p 2220

After that the server ask  a password for authenticity , then we paste the password we copied finally we successfully logged in .

The output of step 2,3 and 4 is here :

<img width="1920" height="1080" alt="read and loggin_3" src="https://github.com/user-attachments/assets/e570d46c-403e-4a01-80b4-730b230bb4bd" />

## What i learned:

        To read the content of file "--spaces in this filename--" we use a command :

        bash:
        cat -- "--spaces in this filename--"
        
        -- indicate that, it tells to the terminal stop processing option , everything after this is a filename. 
        Then the quotation marks keep the spaces together as one filename.

## Platform:
OverTheWire-Bandit
        


