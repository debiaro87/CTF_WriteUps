## Bandit Level 3 → Level 4

# OBJECTIVE 

The main goal of this level is to find the hidden password of bandit level 4 in the "inhere" directory and after getting the password connect to bandit level 4 by using ssh on port 2220.

## 1 Connect to bandit 3:
First we have to connect as bandit 3 to do that we write a command:

bash:

ssh bandit3@bandit.labs.overthewire.org -p 2220

Then it ask us the password of level three since we have it from level 2 we enter it and finally we successfully logged in as bandit 3 server.

The output here below:
<img width="1920" height="1080" alt="Command3" src="https://github.com/user-attachments/assets/e3f960d8-f6ee-4b44-9dd6-70dce22cbecc" />


## 2 check the file :
To check whether the file exist or not we write a command:

bash:

ls

there exist "inhere" but we don't know whether it's file or directory to now that we write the command :

bash:

ls 

then it say's "inhere" is a directory . Well 
<img width="1280" height="800" alt="list" src="https://github.com/user-attachments/assets/b1d8a9d6-eadf-4654-81a9-23e3e7602eb9" />


## 3 Move to inhere directory:
To move to inhere directory we write a command :

bash:

cd inhere

Now we are in "inhere" directory.
<img width="1280" height="800" alt="change direct" src="https://github.com/user-attachments/assets/4022d26f-98f4-4afe-9aaf-1231cb66e35b" />

## 4 check the file:

To know the list of file exist in inhere directory we write a command:

bash:

ls 

You see! we didn't see nothing because it is hidden file . To display the hidden one we write a command:

bash:

ls -la

Know we are sawing a list of files but the hidden one is the one which have ... infront  which is "...Hiding-From-You".
<img width="1920" height="1080" alt="READ3" src="https://github.com/user-attachments/assets/e9b2ff28-4b45-4b48-b185-4b5fe14c32af" />

## 5 read the content of the hidden file:
To read the content of the hidden file we write a command:

bash:

cat ...Hiding-From-You

Finally we get the password ,so we have to copy it for next level

Here is the output;
<img width="1280" height="800" alt="list and read a hidden" src="https://github.com/user-attachments/assets/8285e943-f2db-49d6-a014-8d3c1fcfca2d" />

## 6 connect to bandit level 4:
To connect as bandit 4 , first we have to exit or log out the previous bandit. then after we use ssh on port 2220 to log in bandit 4
<img width="1280" height="800" alt="Exit" src="https://github.com/user-attachments/assets/9ec129cd-8782-4976-b3c4-c3e1f4e8d99c" />

bash:

ssh bandit4@bandit.labs.overthewire.org -p 2220

Then it ask us the password so we have to paste the password we copied here


The output is here below:
<img width="1280" height="800" alt="command 4" src="https://github.com/user-attachments/assets/bf769bd3-7f35-4896-b84c-ffcbe4e4241a" />
finally we logged in as bandit 4 in to the server port 2220

## What i learned :
                  ls       # list normal files
                  ls -a    # list all files, including hidden files
                  ls -l    # detailed information
                  ls -la   # detailed information + hidden files
                  cd       # change directory
                  cat      # display file contents

## Platform:
OverTheWire:Bandit


