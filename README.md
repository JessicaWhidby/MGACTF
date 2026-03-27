The LOLCODE challenge was created purely for fun.
I happened to stumble upon the LOLCODE esoteric programming language while working on other challenges for MGACTF, some of which are included in this repository.
I thought it would be a fun project for myself to try and figure out how the language works and see if competitors could decipher which flag was correct.

The Stego-saurus pt 1 was created using Steghide in Kali Linux. I made several challenges with this tool, including some layered challenges, but I only added one here.
Using steghide embed -cf [image] -ef [secret], I was able to hide the secret file within the cover image.
Therefore, you can undo this using steghide extract -sf [image].
Use password MGACTF.

Stego-suarus pt 2 was created using Stegosuite, also in Kali Linux. This was originally more involved, using clues from previous challenges.
However, here, I simply used stegosuite embed -m "[message]" -o [file to output] -k="MGACTF" [image] 
With -k meaning the key or the password.
To undo this and find the flag, use stegosuite extract -k="MGACTF" [image].
