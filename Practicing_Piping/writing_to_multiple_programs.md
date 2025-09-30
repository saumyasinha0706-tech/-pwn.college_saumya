# Challenge Name
Write to multiple programs

## My solve
**Flag:** `pwn.college{AVn0xZE_VJNaPlizRofFojEIVim.QXwgDN1wCOwEzNzEzW}`
i used output process substitution  with the tee command to duplicate the output of /challenge/hack to both the /challenge/the and /challenge/planet programs.

```bash
 /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
941220751527011677
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{AVn0xZE_VJNaPlizRofFojEIVim.QXwgDN1wCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
i learned output process substitution

## References 
None
