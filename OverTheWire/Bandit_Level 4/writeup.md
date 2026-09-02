## Bandit Level 3 → Level 4

# OBJECTIVE 

The main goal of this level is to find the hidden password of bandit level 4 in the "inhere" directory and after getting the password connect to bandit level 4 by using ssh on port 2220.

## 1 Connect to bandit 3:
First we have to connect as bandit 3 to do that we write a command:

bash:

ssh bandit3@bandit.labs.overthewire.org -p 2220

Then it ask us the password of level three since we have it from level 2 we enter it and finally we successfully logged in as bandit 3 server.

## 2 check the file :
To check whether the file exist or not we write a command:

bash:

ls

there exist "inhere" but we don't know whether it's file or directory to now that we write the command :

bash:

ls 

then it say's "inhere" is a directory . Well 

## 3 Move to inhere directory:
To move to inhere directory we write a command :

bash:

cd inhere

Now we are in "inhere" directory.
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






