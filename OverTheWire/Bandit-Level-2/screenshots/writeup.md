## Bandit Level 1 → Level 2

# OBJECTIVE
The main goal of this level is to find the password of bandit level 2 in the "-" file that exist in  home directory. 

After finding the password , use it to log in to "bandit level_2" account by using ssh on port "2220"
## To solve this we pass through three steps:
## step 1: logging in to bandit_1:

First we have to log in as bandit_1 in to the server, to do that we write a command :

bash:

SSH bandit1@bandit.labs.overthewire.org -p 2220

The very important part is:

<img width="1280" height="800" alt="Command_1" src="https://github.com/user-attachments/assets/c0ca9f27-779f-4da6-b038-24af2029114e" />


After that,it ask as the password to authenticity, since we have a password we get in level 0 from a file "readme" we enter that password then we successfully  logged in as bandit_1 

## step 2 check the file:
To identify whether the file exist or not  in the home directory we use the command:

bash:

ls

so the filename  called "-" is  exist home directory

## step 3 read the content of the file:
To read the content of the file called "-" we use the command :

bash:

cat ./-

To avoid the terminal took "-" file to another option we use ./ infront of it that mean :

./ ~ show current directory and

- ~ shows file name

after we enter the enter key we get the password which exist in the "-" file

remember : to use ./ infront of symbols file name

## step 4 connect to bandit level 2:
To connect as bandit 2 we first exit the first bandit server and we connect by using ssh on port 2220 and the password we get from "-" file in bandit 1 server

bash:

ssh bandit2@bandit.labs.overthewire.org -p 2220

and it ask us the password then we enter the password we get from bandit1 "-" file finally we logged in as a bandit2 server 

Look at this image and understand:

<img width="1280" height="800" alt="read and loggin_2" src="https://github.com/user-attachments/assets/ec49b4b8-a098-4de3-82d2-ad9ee432d32c" />


# what i learned:
          When we want to read the files that named in symbol we have to tell to the terminal first as we are in the directory unless it take as another option and error is occured
# Note:

Remember always to log out or exit the bandit server you are in first before to connect as another bandit

## Platform:

OverTheWire: bandit



