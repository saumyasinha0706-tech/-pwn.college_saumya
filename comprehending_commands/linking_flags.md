# Challenge Name
Linking files

## My solve
**Flag:** `pwn.college{c0BKEsDICpAmoeMUAIjYKJ8u4HP.QX5ETN1wCOwEzNzEzW}`
I followed the instructions from the challenge.

```bash
 cat /challenge/catflag
#!/opt/pwn.college/bash

fold -s <<< "About to read out the /home/hacker/not-the-flag file!"
cat /home/hacker/not-the-flag
hacker@commands~linking-files:~$ rm -f ~/not-the-flag
hacker@commands~linking-files:~$ ln -s /flag ~/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{c0BKEsDICpAmoeMUAIjYKJ8u4HP.QX5ETN1wCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned about linking files

## References 
None
