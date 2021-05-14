# Bandit Level 10 to 11 Writeup

Author: [Harsh Jain](https://github.com/Harshj20) 

Problem Page: [bandit11](https://overthewire.org/wargames/bandit/bandit11.html)

## List of Commands Used
```
ls - list files in a directory
base64 - base64 encode/decode data and print to standard output

```

## Walkthrough
How did you solve this level? Include the complete thought process, even stuff that didn't work. Give explanations wherever necessary.
First few steps were common - using *ssh* to connect to the remote machine and then doing *ls* to look for the file *data.txt*.
Its answer was right in the Question. I looked up the manpage of *base64*. Straightforward Question. 

## Password
`IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`

## Bash/Python script to automate the process
```
#!/usr/bin/bash

sshpass -p truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk ssh bandit10@bandit.labs.overthewire.org -p 2220 << hi
base64 -d data.txt | tr ' ' '\n' | tail +4
exit
hi

```

## Suggested modifications [Optional]
What can you do to make this level more difficult. The inherent idea should be similar.
