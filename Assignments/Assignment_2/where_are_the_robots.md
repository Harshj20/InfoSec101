# PicoGym Web Exploitation Writeup


Author: [Harsh Jain](https://github.com/Harshj20) 

Challenge Page: [Where are the robots](https://jupiter.challenges.picoctf.org/problem/3647)

## Walkthrough
How did you solve this level? Include the complete thought process, even stuff that didn't work. Give explanations wherever necessary.
The name suggested that it had something to do with the robots.txt file (I learnt about this in one of the previous challenges. So I just added /robots.txt in the domain and it redirected
me to new page showing the info -
```
User-agent : *
Disallow: /477ce.html
```
This prompted me to look for the file '/477ce.html' as it was like a path. So I added this path to the initial domain and Voila!
## Flag
`picoCTF{ca1cu1at1ng_Mach1n3s_477ce}`

## Useful resources (if any)

## Suggested modifications [Optional]
What can you do to make this level more difficult. The inherent idea should be similar.
