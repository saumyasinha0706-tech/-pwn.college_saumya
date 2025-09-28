# Challenge Name
Making directories

## My solve
**Flag:** `pwn.college{Yg4Mq4XjLw2rd2GuS8HHe81mBpl.QXxMDO0wCOwEzNzEzW}`
I followed the instructions in the challenge to make a directory.

```bash
 mkdir /tmp/pwn
hacker@commands~making-directories:~$ touch college
hacker@commands~making-directories:~$ /challenge/run
Uh oh! /tmp/pwn/college does not exist. Please use the 'touch' command to
create it!
hacker@commands~making-directories:~$ touch /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{Yg4Mq4XjLw2rd2GuS8HHe81mBpl.QXxMDO0wCOwEzNzEzW}
```
## Incorrect tangents I went on
I forgot to use the 'touch' command to
create /tmp/pwn/college

## What I learned
I learned how to make directories

## References 
None
