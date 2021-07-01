# Password

656565656565656565656565656565654644 (in hex)

# Approach

After 'main', I explored the 'login' function, and then 'test_password_valid'. But nothing fruitfull came out. But the Login function was a bit suspicious as this time my password was not stored at memory location 0x2400.
Also after I used 'aaaaaaaaaaaaa' as a random password, some instruction got overwritten. 
I was not getting any lead so i checked some writeups for this level.
I found one very good writeup where I got to learn about some new things like 'Buffer overflow' and all.
In this level we are exploiting buffer overflow to overwrite the return address of login and change it to the addres of 'unlock door' function.   

