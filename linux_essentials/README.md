# Task1.Part1 
## 1) Log in to the system as root.  
```console
##switch to administrator without changing the current directory
student@CsnKhai:~$ sudo -s
#switch to admin (#)
student@CsnKhai:~$ sudo su
```
## 2) Use the passwd command to change the password. Examine the basic parameters of the command. What system file does it change?
```bash
#change user password
passwd user_name
#basic parameters 
#delete user password
-d
#make the password obsolete
-e
#lock the account if the user has not changed the password in n days
-i n 
#the maximum number of days n that the user's password is valid
-x n
#the number of days n after which to display a message about the need to change the password 
-w n 
```
The passwd command changes some of the entries in the /etc/passwd file.

## 3) Determine the users registered in the system, as well as what commands they execute. What additional information can be gleaned from the command execution? 

## 4) Change personal information about yourself.
```bash
#change personal information displayed by finger
chfn
#change your login shell
chsh
#change the user's password
passwd
```

## 5) Become familiar with the Linux help system and the man and info commands. Get help on the previously discussed commands, define and describe any two keys for these commands. Give examples. 
```bash
Command info gives more detailed information about the command rather than man.
```

```console
#Usage of man:
student@CsnKhai:~$ man passwd
#Usage of info:
student@CsnKhai:~$ man passwd

#Part of result:
-a, --all
           This option can be used only with -S and causes show status
           for all users.

-d, --delete
           Delete a user`\`s password (make it empty). This is a quick way
           to disable a password for an account. It will set the named
           account passwordless.

```

## 6) Explore the more and less commands using the help system. View the contents of files .bash* using commands. 
```console
#Usage of help to find out what command about:
student@CsnKhai:~$ less --help
```
```console
#Usage of less:
student@CsnKhai:~$ less --help.bash*
```
<img id="theImage" src="./picture/less.jpg">

```console
#Usage of more:
student@CsnKhai:~$ less --help.bash*
```
## 7) * Describe in plans that you are working on laboratory work 1. Tip: You should read the documentation for the finger command. 

## 8) * List the contents of the home directory using the ls command, define its files and directories. Hint: Use the help system to familiarize yourself with the ls command. 