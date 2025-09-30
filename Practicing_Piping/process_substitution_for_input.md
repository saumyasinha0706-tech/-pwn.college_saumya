# Challenge Name
Process substituition for input

## My solve
**Flag:** `pwn.college{I6TKfpf1-naxqJCdns7tO7nBvQk.0lNwMDOxwCOwEzNzEzW}`
i used diff with process substitution to compare the outputs of /challenge/print_decoys and /challenge/print_decoys_and_flag.

```bash
diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
1a2
> pwn.college{I6TKfpf1-naxqJCdns7tO7nBvQk.0lNwMDOxwCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned about process substitution

## References 
None
