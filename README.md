OBJECTIVE</br>
Middle Georgia State University hosted a conference, and the student-led Cyber Knights cyber defense competition team created a CTF for anyone attending to participate in. Challenges had a wide range of difficulty and included areas such as code analysis and steganography (shown here), as well as things like network traffic analysis, web app exploitation, digital forensics, and cryptography.

TOOLS USED</br>
My challenges shown here used a simple text editor (to create the LOLCODE challenge) and various steganography tools like Digital Invisible Ink Toolkit, Stegosuite, and Steghide; the latter 2 of which are Linux CLI tools.

KEY TAKEAWAYS</br>
Creating all of these challenges was a challenge in itself for all of us. We had a lot of interesting discussions surrounding how exactly to create these and make them fun, educational, and engaging for the audience. I learned how to properly write up a question that can be asked, how to solve everyone's challenges from scratch (other challenges included cryptography, Wireshark analysis, and web app exploitation), and how to understand the perspective of someone else who may be trying to solve these challenges with no prior knowledge (ensuring that they got progressively more difficult, but still very possible for a beginner). I especially learned a lot from the LOLCODE code analysis question I created, as I not only had to learn a whole new programming language, but also how to incorporate it into a puzzle that can be solved. I also enjoyed learning the steganography tools as I had never used any of them prior to creating these challenges. Steganography has always been intriguing to me, so being able to apply the concepts was very interesting and fun.

I believe all of these skills can transfer to a blue team role. For example, I learned a lot of soft skills in the process, like thinking through a problem from other persepctives. Looking at things from the perspective of a coworker could help me understand why they came to certain conclusions, while looking at things through the lens of an attacker is a crucial skill in determining how they may have gotten and kept access, and where to look for evidence of such.

LOLCODE CODE ANALYSIS CHALLENGE</br>
The LOLCODE challenge was created purely for fun. I happened to stumble upon the LOLCODE esoteric programming language while working on other challenges for MGACTF, some of which are included in this repository.
I thought it would be a fun project for myself to try and figure out how the language works and see if competitors could decipher which flag was correct.

STEGO-SAURUS PT 1</br>
This one was created with Steghide in Kali Linux. As I mentioned before, steganography just captures my attention and I enjoy the puzzles associated with the concept.

STEGO-SAURUS PT 2</br>
Stego-saurus pt 2 was created using Stegosuite, also in Kali Linux. This was also originally more involved, using clues from previous challenges. However, here, I have simplified it a bit so it can be solved without that prior knowledge.

MGASIGN.BMP</br>
MGAsign.bmp uses yet another steganography tool, the Digital Invisble Ink Toolkit. This is a Windows GUI-based tool, so it should be pretty simple to retrieve the message here.
I did create one with a password that had to be found later in the CTF, but that one was a bit more involved and would be more difficult to explain the entire process here.
