# Challenge Name
Hidden files

## My solve
**Flag:** `pwn.college{Ay4kAeAAwouINs-IEOCb-kbWUtK.QXwUDO0wCOwEzNzEzW}`
The challenge asked to change to / directory and then i would have to find a hidden file. clearly that meant i had to use ls -a. i found the file name and then i catted it to obtain flag.

```bash
 cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv           bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-8042508827353  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat flag-8042508827353
cat: flag-8042508827353: No such file or directory
hacker@commands~hidden-files:/$ cat .flag-8042508827353
pwn.college{Ay4kAeAAwouINs-IEOCb-kbWUtK.QXwUDO0wCOwEzNzEzW}
```
## Incorrect tangents I went on
I forgot to add . before the flag file name.

## What I learned
I learned about hidden files and how to access them,

## References 
None
