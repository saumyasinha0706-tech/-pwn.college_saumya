# Challenge Name
Exporting variables

## My solve
**Flag:** `pwn.college{gpSEdeTh1zoYfxmB7L7g6fEmUq7.QXyYTN0wCOwEzNzEzW}`
i first set the pwn variable to college and exported it, making it available to the challenge script. then, i set the college variable to pwn without exporting it.then, i did /challenge/run.
```bash
 export PWN=COLLEGE
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{gpSEdeTh1zoYfxmB7L7g6fEmUq7.QXyYTN0wCOwEzNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```
## Incorrect tangents I went on
None

## What I learned
I learned about exporting variables.

## References 
None
