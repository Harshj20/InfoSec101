# Password

36263b4023623e47 (in Hex)

# APPROACH

As usual, I Started with 'main'. The element which was worth inspecting was 'check password' at 0X444c.
As New orleans, the password here too was hardcoded.
In the New orleans level, I had Googled the use of 'mov.b' after which I got to know that .b suffix is used for byte operation and if .b suffix in not present then word operation is done.
Then I googled about word operation and from there, the meaning of little and big endian.
After this, the level was as simple as the 'New orleans'.At first, the endian part didn't strike me and I had no idea the MSP430 was little endian and thus it longer than usual time to clear this level.
