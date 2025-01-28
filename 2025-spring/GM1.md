# GM 1: Hack the Playground

Technologies used: PowerShell, netcat, terminal, Burp Suite, Ghidra, Python, JavaScript, cryptography, Go

## 1. Tag: Let Me Play
<img width="723" alt="image" src="https://github.com/user-attachments/assets/9dfbcdd5-8b42-47aa-b9d0-ec3794873f4d" />

Method: Go to the NEU CTF instagram account, navigate to the linktree, click on the Discord link, and find the invite code in the URL bar.

Flag: CTF{https://discord.com/invite/4B2CmPZvC7}


## 2. Minesweeper
<img width="714" alt="image" src="https://github.com/user-attachments/assets/fcf2ece7-7614-478b-9013-81cbab37faf6" />

Method: Solve the game of Minesweeper using the usual rules. We can see that the number 3 at (8,5) is only touching 2 flags and the number 2 at (8,4) is only touching 1 flag, so the flag should be planted at (9,5).

Flag: CTF{(9,5)}


## 3. Where's Waldo?
![image](https://github.com/user-attachments/assets/53f62043-a502-4383-a0c2-e3f87fcbd3c1)
Method: Reverse image seach the image to find the location.
Flag: CTF{SOUTHBEACH}

## 4. Memory
<img width="707" alt="image" src="https://github.com/user-attachments/assets/a21d6aef-b0b7-4ab0-9513-bd99e7bedeab" />

Method: First, I saw that 2 ciphertexts both start with the number 63. This must correspond to the letter C in "crack" and "codes".
Then, I saw that one ciphertext has 63 again, which must be the second c in "crack". We now know that box 5 is the word "crack" and box 9 is the word "Codes".
From the ciphertext for "Crack" we know that the letter "a" is the number 61. Box 4 also has the number 61 so it must be "flags". Therefore, box 3 is the word "seize".

Flag: CTF{5934}


## 5. Passing Notes
<img width="710" alt="image" src="https://github.com/user-attachments/assets/f45839d0-3e5b-4db2-b65c-866acdcf9df4" />
<img width="542" alt="image" src="https://github.com/user-attachments/assets/1453d545-218c-4fcc-abf8-efee9d2a38e2" />
<img width="157" alt="image" src="https://github.com/user-attachments/assets/844bb78c-db80-4eef-8b43-64df4624c08e" />

Method: Examine the code to see that the code is simply performing a bitwise XOR operation on the input and outputting it to a file. Based on the properties of XOR, we know that we can flip the input and output to get the plaintext.
I edited the code file to switch the input and output files, than ran the program using PowerShell then opened the output file to find the flag.

Flag: CTF{g1ve_m3_ur_cod3!}


## 6. Hide n Seek: Hiding Monster
<img width="677" alt="image" src="https://github.com/user-attachments/assets/d980a129-fb82-4bee-b628-1f088267049f" />
<img width="744" alt="image" src="https://github.com/user-attachments/assets/2ba01d56-5de5-4dc6-9680-acd7e2ac0ff6" />

Method: I opened the developer tools of the website then went to storage then cookies to find the CTF stored as a cookie value.

Flag: CTF{C00KIEM0NST3R}


## 7. Mother, May I?
<img width="430" alt="image" src="https://github.com/user-attachments/assets/efdd224e-6ed5-4e49-b98c-3104f59563e3" />
<img width="854" alt="image" src="https://github.com/user-attachments/assets/6b8b2676-5dee-4771-85a4-01a4d1ef3d35" />
<img width="566" alt="image" src="https://github.com/user-attachments/assets/10993c17-c7b8-47c3-86fb-31af168591b2" />

Method: By reading the Mother.py file we can see the program logic that the flag will be revealed if our command contains the words "flag" and "please".
Connect to the server using netcat then enter "flag please" to get the flag.

Flag: CTF{m00oooo00000oooooommmmm}


## 8. Four-Square
<img width="641" alt="image" src="https://github.com/user-attachments/assets/dc2bc479-4241-4943-8f69-9eddd5aff5d0" />
<img width="333" alt="image" src="https://github.com/user-attachments/assets/ebbf485c-89cd-4ca6-ad18-6984eb1f10de" />

Method: I recognized the four square cipher so I opened up the dcode.fr solver, set it to the four square cipher, then entered in the message.

Flag: CTF{FOURSQUAREISCOOLWITHMATH}


## 9. Tic tac toe
<img width="428" alt="image" src="https://github.com/user-attachments/assets/1a68cb83-1eef-4e82-ab92-7c3362abfe9d" />
<img width="1147" alt="image" src="https://github.com/user-attachments/assets/d8f8aa0e-9d27-4454-81a3-2a1cb1729a75" />

Method: I opened the game website in Burp Suite to intercept the HTTP requests. When the computer was about to make the game winning move, 
I changed the HTTP packet to modify the board state in game so I would win.

Flag: CTF {t1c_t4c_f33t}


## 10. 20 Questions
<img width="546" alt="image" src="https://github.com/user-attachments/assets/23f90ae0-a69d-4544-aefa-dc3f3c62be13" />
<img width="1310" alt="image" src="https://github.com/user-attachments/assets/51655ed7-1b0c-4638-8400-2c4808547dda" />

Method: I opened the stripped file in Ghidra then examined the decompiled code in function 001011a9 to see that the obfuscated byte array is being XOR'd with 0x29. I simply XPR'd it with 0x29 again to get the flag.

Flag: CTF{20_w4s_t00_f3w!}


## 11. Hopscotch
<img width="720" alt="image" src="https://github.com/user-attachments/assets/0a71acc6-24a1-456d-a697-0a07c87196ab" />
<img width="740" alt="image" src="https://github.com/user-attachments/assets/70a05128-b1f7-443c-8826-69d7b447a332" />
<img width="742" alt="image" src="https://github.com/user-attachments/assets/fdc199f6-f624-4015-a6a5-c6340f16bd3c" />
<img width="728" alt="image" src="https://github.com/user-attachments/assets/92e72314-7945-4178-9f9a-a2aac4680e61" />
<img width="743" alt="image" src="https://github.com/user-attachments/assets/b9acca79-6069-4f6c-8a32-d6a864474fdd" />
<img width="493" alt="image" src="https://github.com/user-attachments/assets/e25c0530-d0c5-4b63-9615-7118abb2fc3f" />
<img width="744" alt="image" src="https://github.com/user-attachments/assets/e207a39f-25bf-4c39-879c-76bd98a43cc1" />
<img width="494" alt="image" src="https://github.com/user-attachments/assets/18af1d61-8789-48ae-b40b-7336e0a4abe0" />

Method: I used the developer tools to find hidden messages in the HTML, CSS, and JS files which allowed me to figure out the flag.
The final hop involves deobfuscating JS code then running it to find the final URL path.

Flag: CTF{y0u_rule_th3_playgr0und_now}


## 12. Rock Paper Scissors: Deathmatch Edition!
<img width="697" alt="image" src="https://github.com/user-attachments/assets/abd7a162-aea7-4116-958f-1deafc36f26c" />
<img width="771" alt="image" src="https://github.com/user-attachments/assets/65b9ace9-28c7-4796-ad36-32eaa7cb2714" />

Method: In order to beat the opponent I wrote a python script which reads the opponent's next move then counters with the correct move.
I ran the program to interact with the nc gm.neu-ctf.club 11110.

Flag: CTF{rps_victory_1snt_gu4rant33d}


## 13. Simon Says
<img width="691" alt="image" src="https://github.com/user-attachments/assets/a76fe95c-b6d2-4311-a858-f47825cd4e85" />
<img width="741" alt="image" src="https://github.com/user-attachments/assets/ebe40318-31af-4263-a15b-55e77c5cfb06" />

Method: This is a simple time trial that involves decoding the given ciphertext with the appropriate cipher using dcode.fr in the alloted time to get the flag.

Flag: CTF{S1m0N_s4Yz_@_L0t}


## 14. Hangman
<img width="409" alt="image" src="https://github.com/user-attachments/assets/6aa25065-41cc-41dd-8b93-2876193f2734" />
<img width="1493" alt="image" src="https://github.com/user-attachments/assets/75f904f5-8fc4-4e1f-869e-bc4514bd9347" />

Method: I decompiled the Go code in ghidra to see the program logic, then patched the appropriate game control code to always jump to the win condition to obtain the flag.

Flag: CTF{this_isnt_fun}
