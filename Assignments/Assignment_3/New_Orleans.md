# PASSWORD

`w6cE}oW`

# APPROACH

At first, I inspected the 'main' function. At the second instruction there was a call to a function called
'create password'. So I hopped to explore it. It was clear that the password was hardcoded for memory address
0x2400. So I added a breakpoint at the 'ret' of the 'create password' function. Then I ran the program 
checked the live Memory Dump. There was my password starting from memory address 0x2400.
