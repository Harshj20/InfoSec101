# PicoGym Web Exploitation Writeup


Author: [Harsh Jain](https://github.com/Harshj20) 

Challenge Page: [Cookies](http://mercury.picoctf.net:27177/)

## Walkthrough
How did you solve this level? Include the complete thought process, even stuff that didn't work. Give explanations wherever necessary.
At first, I google searched about Cookies. After learning some info about its types, its use, how to access them, I jumped to the 
link and found a cookie, using Developer tools, with its Name value set to -1. So I changed its value to 0 and reloaded the site 
which now displayed something new. This prompted me to change the Name values. I went from 0 to 6-7 and everytime It displayed something new
but not the flag. So I decided to automate the task using bash script.
```
#!/usr/bin/bash
for i in {1..20}
do
    curl -b "name=$i" "http://mercury.picoctf.net:27177/check"
done
```
The range 1-20 was random. It displayed a lot of information so I piped the output with `grep -w "picoCTF"`.
## Flag
`picoCTF{3v3ry1_l0v3s_c00k135_064663be}`

## Useful resources (if any)

## Suggested modifications [Optional]
What can you do to make this level more difficult. The inherent idea should be similar.
