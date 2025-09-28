# Challenge Name
Multiple options for tab completion

## My solve
**Flag:** `pwn.college{Uzjc10TV_EATU7gryNHJRPT6Dck.0lN0EzNxwCOwEzNzEzW}`
I typed cat /challenge/files/pwn but since there were multiple files starting from pwn, i pressed tab multiple times. i got the list for all files where i found the flag, which i accessed to obtain the flag.

```bash
 cd /challenge/files
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ cat /challenge/files/pwn
pwn                    pwncollege-family      pwncollege-flyswatter
pwn-college            pwncollege-flag        pwncollege-hacking
pwn-the-planet         pwncollege-flamingo
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ cat /challenge/files/pwncollege-flag
pwn.college{Uzjc10TV_EATU7gryNHJRPT6Dck.0lN0EzNxwCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned more about tab completion.

## References 
None
