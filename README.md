Creating all of these challenges was a challenge in itself for my team and me. We had a lot of interesting discussions surrounding how exactly to create these and make them fun, educational, and engaging for the audience. I learned how to properly write up a question that can be asked, how to solve everyone's challenges from scratch (other challenges included cryptography, Wireshark analysis, and web app exploitation), and how to understand the perspective of someone else who may be trying to solve these challenges with no prior knowledge (ensuring that they got progressively more difficult, but still very possible for a beginner). I especially learned a lot from the LOLCODE code analysis question I created, as I not only had to learn a whole new programming language, but also how to incorporate it into a puzzle that can be solved. I also enjoyed learning the steganography tools as I had never used any of them prior to creating these challenges. Steganography has always been intriguing to me, so being able to apply the concepts was very interesting and fun. All in all, helping to create this CTF that we hosted for other IT students was a great learning experience, both in application of concepts and in teamwork and collaboration.

With that being said, here is an explanation of how to solve each challenge!

The LOLCODE challenge was created purely for fun.
I happened to stumble upon the LOLCODE esoteric programming language while working on other challenges for MGACTF, some of which are included in this repository.
I thought it would be a fun project for myself to try and figure out how the language works and see if competitors could decipher which flag was correct.
The answer is MGACTF{NO WAY:)I NOT UR KITTEH}, which isn't so bad to figure out once you decipher how the language works with if statements.

The Stego-saurus pt 1 was created using Steghide in Kali Linux. I made several challenges with this tool, including some layered challenges, but I only added one here.
Using _steghide embed -cf [image] -ef [secret]_, I was able to hide the secret file within the cover image.
The _cf_ stands for _cover file_, or the photo that will contain the secret. Thus, _ef_ stands for _embed file_, or the secret that is put inside of the cover file. 
With this in mind, you can undo this using _steghide extract -sf [image]_.
Here, _sf_ would be _stegofile_, the file with the steganographic text hidden inside of it.
Use password MGACTF. The original password was based on the flavortext of the challenge and previous challenges, but I recreated it with the MGACTF password for simplicity here.

Stego-saurus pt 2 was created using Stegosuite, also in Kali Linux. This was also originally more involved, using clues from previous challenges.
However, here, I simply used _stegosuite embed -m "[message]" -o [file to output] -k="MGACTF" [image]_.
With _-k_ meaning the key or the password.
To undo this and find the flag, use _stegosuite extract -k="MGACTF" [image]_.

MGAsign.bmp uses yet another tool, the Digital Invisble Ink Toolkit. This is a Windows GUI-based tool, so it should be pretty self-explanatory to retrieve the message here. Just
use the Decode tab, select a path for the message to be output to, and go. There is no password for this one. I did create one with a password that had to be found, but that one was a bit more involved and would be more difficult to explain the entire process here.
