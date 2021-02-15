# WalkThrough 
## Linux Fundamentals 3 Part-1

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



