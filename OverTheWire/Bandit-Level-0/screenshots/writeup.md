## OverTheWire Bandit level 0

# Objective
The goal of this level was to login in to OverTheWire game server using ssh.
# The provided connection information was:
            host:"bandit.labs.overthewire.org"
            port:2220
            username:bandit0 and 
            password:*********
# Tools used:
            SSH
            Linux terminal
# Solution:
I used SSH to connect to remote bandit server.
a command format was:
bash:
  ssh username@host -p port 
==============================================
using the provided information i ran:
bash:
ssh bandit0@bandit.labs.OverTheWire.org -p 2220
===============================================
and after that 
The first time I connected ,ssh displayed the message asking me to verify the authenticity of the host.
I confirmed the connection by typing the text:

"yes"
SSH then asked for the password. I entered the provided password and finally successfully I logged in to the bandit server.

# Command used:

bash:
ssh bandit0@bandit.labs.OverTheWire.org -p 2220

# what I learned is:
