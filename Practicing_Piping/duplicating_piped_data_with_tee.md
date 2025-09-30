# Challenge Name
Duplicating piped data with tee

## My solve
**Flag:** `pwn.college{IUX3ve-4eaf5NkdNjfzHrAbDlOf.QXxITO0wCOwEzNzEzW}`
i looked for a filename that would have the secret code. i catted the path to get the secret code. then i piped the data using tee

```bash
 cd ~
hacker@piping~duplicating-piped-data-with-tee:~$ ls
COLLEGE  PWN  a  college  instructions  myflag  not-the-flag  pwn  pwn_out  temp_file  the-flag
hacker@piping~duplicating-piped-data-with-tee:~$ cd /tmp
hacker@piping~duplicating-piped-data-with-tee:/tmp$ ls
bin  hsperfdata_root  tmp.4mK6TfTSUV
hacker@piping~duplicating-piped-data-with-tee:/tmp$ cd ~
hacker@piping~duplicating-piped-data-with-tee:~$ cat /pwn_out
cat: /pwn_out: No such file or directory
hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn_out
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "IUX3ve-4"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret IUX3ve-4 | tee /tmp/pwn_out | /challenge/colleg
e
Processing...
^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[CCorrect! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{IUX3ve-4eaf5NkdNjfzHrAbDlOf.QXxITO0wCOwEzNzEzW}
```
## Incorrect tangents I went on
i had trouble finfing the filename at first and then made some syntax errors.

## What I learned
I learned about the tee command.

## References 
None
