# Challenge Name
Exclusionary globbing

## My solve
**Flag:** `pwn.college{4wUlILGM3T0iWqK_xic_2UYZgbt.QX2IDO0wCOwEzNzEzW}`
i had to finf all files that didnt start with p,w,n which meant i had to use !,[],*

```bash
 cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{4wUlILGM3T0iWqK_xic_2UYZgbt.QX2IDO0wCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned about globs that can filter out content. 

## References 
None
