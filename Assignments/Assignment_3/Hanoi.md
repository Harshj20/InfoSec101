# Password

65656565656565656565656565656517 (in hex)

# Approach

After inspecting 'main', I took a look at 'login' function. It was clear that my input is stored from 0x2400.
The unlock door function is called if the condition is met at 0X455a which is `cmp.b #0x17, &0x2410`. So I used the above mentioned password in which
the first 15 char are absolutely random and the 16th char is 0X17.
The door got unlocked. After some more testing, It was made clear that the password had to be atleast 16 char long in which the 16th char should be 0x17. 
