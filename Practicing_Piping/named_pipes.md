# Challenge Name
Named pipes

## My solve
**Flag:** `pwn.college{wzGQskK3AL-FeRAILGIZTXJBqWL.01MzMDOxwCOwEzNzEzW}`
I created a FIFO and then redirected the output of /challenge/run to /tmp/flag_file

```bash
 mkfifo /tmp/flag_fifo
mkfifo: cannot create fifo '/tmp/flag_fifo': File exists
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{wzGQskK3AL-FeRAILGIZTXJBqWL.01MzMDOxwCOwEzNzEzW}
pwn.college{wzGQskK3AL-FeRAILGIZTXJBqWL.01MzMDOxwCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
We can also create your own persistent named pipes that stick around on the filesystem! These are called FIFOs, which stands for First (byte) In, First (byte) Out.


## References 
None
