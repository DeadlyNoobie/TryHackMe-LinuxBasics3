# WalkThrough 
## Linux Fundamentals 3 

**Deploy the machine**

**SSH into the machine with given cred**

```
    sudo ssh shiba3@ip 
```

**Go Through cp Command**

**cd and relative paths**

_home_

```
cd ~
```
Making directory called test in /tmp

```
mkdir /tmp/test
```
**Read ln basics**

How would I link /home/test/testfile to /tmp/test

```
ln /home/test/testfile /tmp/test
```
How do you find files that have specific permissions?

[Find Files based on Perms](https://ostechnix.com/find-files-based-permissions/)

```
-perm
```



How would you find all the files in /home

```ssh
find /home
```



How would you find all the files owned by paradox on the whole system

[Find permissions](https://www.cyberciti.biz/faq/how-do-i-find-all-the-files-owned-by-a-particular-user-or-group/)

```
find / -user paradox
```

What flag lists line numbers for every string found?

[grep getlinenumber](https://stackoverflow.com/questions/3213748/get-line-number-while-using-grep)

```
-n
```

How would I search for the string boop in the file aaaa in the directory /tmp

```
grep boop /tmp/aaaa

grep <string> <file>
```

### Task 7



What is shiba4's password

**As told we have to search the binary**

```
find / -name shiba4 -type f 2>>/dev/null
```

[2>>/dev/null why?](https://askubuntu.com/questions/350208/what-does-2-dev-null-mean)

**Now we found two files one of them is interesting**

**Nice we found the Password and we are good to go to shiba4**


### Task 9 Sudo



How do you specify which user you want to run a command as.

```
-u
```
We can look up man page for sudo.



How would I run whoami as user jen?

```
sudo -u jen whoami
```
The question is quite simple we just have to use the -u flag.

[Sudo command ](https://linuxize.com/post/sudo-command-in-linux/)

The above site Linuxize is great site to learn about different commands check it out.

How do you list your current sudo privileges(what commands you can run, who you can run them as etc.)    

```
-l
```



How would I add the user test to the group test

**As already told we need to use sudo in certain conditions for doing big things haha**

```
sudo usermod -a -G test test

sudo usermod -a -G <group name> <user>
```

### Task 11 nano


**Task 11 is all about the nano and it's quite useful go through the entire text and make sure you know how to use it as we will be using it quite frequently**

### Task 12 Shell Files

**We are introduced with the basics of how to execute multiple commands at one time we can do this in more better way using shell scripts which we will take a look later on.**

### Task 13 Directory structure

**This section introduces us to how files are distributed in kali linux and how and where you can find certain files you will be needing on the daily basis.**

### Task 14 apt

**This section introduces how we can do updates in our system and how we can install packages and programmes on our linux system.**

### Task 15 ps

**This command is usful but not used on the daily basis. You can view the man page of this command and further you can also look up online.**



## End of LINUX FUNDAMENTALS PART 3
