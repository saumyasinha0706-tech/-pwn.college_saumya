# Challenge Name
Helpful Programs

## My solve
**Flag:** `pwn.college{4BnSgVIQTLHFUrfoheF3kRKX5vq.QX3IDO0wCOwEzNzEzW}`
i used the --help argument to get the clues. using the clues, i got the secret number, and then the clue.

```bash
/challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge --print-value
The secret value is: 435
hacker@man~helpful-programs:~$ /challenge/challenge -g 435
Correct usage! Your flag: pwn.college{4BnSgVIQTLHFUrfoheF3kRKX5vq.QX3IDO0wCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned about --help argument

## References 
None
