# GM 2: Red Envelope Riddles

Technologies: binary, Python, Python3, VirusTotal, terminal, JavaScript injection, digital forensics, scanmem

## 1. Pattern Recognition 
<img width="809" alt="image" src="https://github.com/user-attachments/assets/ec721cb3-134c-4c18-a623-130809b88f33" />

Method: Simply input the binary code into a converter to get the flag.

Flag:CTF{ssssuper_secret}


## 2. Geolosnake
<img width="922" alt="image" src="https://github.com/user-attachments/assets/91c47860-3fd9-4e68-b5f0-d1b9b2adec49" />

Method: Simply complete the Toy Story quote.

Flag: CTF{boot}


## 3. Ancient Antidote
<img width="908" alt="image" src="https://github.com/user-attachments/assets/98979678-3f8b-4402-8a12-d656a56eff16" />
<img width="420" alt="image" src="https://github.com/user-attachments/assets/d6b4856b-ca84-4f5d-9507-ee3193dd3410" />
<img width="148" alt="image" src="https://github.com/user-attachments/assets/37f5261f-7368-4e2c-949e-2b2a136fc049" />

Method: I reverse engineered the Python code and wrote code to decypt the secret message.

Flag: CTF{w4lk_it_0ff}


## 4. Totally Lucky
<img width="903" alt="image" src="https://github.com/user-attachments/assets/290d1d42-e224-4c12-913e-f091d9521a72" />
<img width="988" alt="image" src="https://github.com/user-attachments/assets/23167305-0d08-4baf-a4ad-f2f9378c49e5" />

Method: I searched the malicious file hash using VirusTotal then navigated to the relations tab to find the contacted URL.

Flag: CTF{http://ttgholidays.com/s.png}


## 5. Slithery
<img width="905" alt="image" src="https://github.com/user-attachments/assets/4b04b577-94cf-4b5e-b7fd-caa11e0ebe54" />
<img width="721" alt="image" src="https://github.com/user-attachments/assets/38ec8f79-b8e1-4289-9df3-bcb725fafa89" />

Method: I again reverse engineered the python code to write a decryption function and entered the code to get the flag.

Flag: CTF{SL1TH3RY_SN4K3}


## 6. Shrink
<img width="898" alt="image" src="https://github.com/user-attachments/assets/cc49ad8b-0f3b-4d47-ad62-8443e16b26c3" />
<img width="399" alt="image" src="https://github.com/user-attachments/assets/10b96b51-3c5d-4933-8028-34fe580b4c9b" />

Method: I used the terminal "file" command to figure out the file type of the shrink file. After seeing that it was a tar file, I used tar and gzip commands to unzip the file to get the flag.

Flag: CTF{EXPANDDDDDDDDDDDD}


## 7. The Slippery Snake
<img width="927" alt="image" src="https://github.com/user-attachments/assets/d10c82f6-c0d3-4bc5-9ab4-42da510c527f" />
<img width="638" alt="image" src="https://github.com/user-attachments/assets/9ff7dcda-d6e9-4016-a4f4-f0b2f144d159" />
<img width="1472" alt="image" src="https://github.com/user-attachments/assets/36abe95e-8028-404e-b647-5d50e61666da" />

Method: I investigated the application logs to see that the vulnerability invovled a YAML desearialization error. I searched Miitre's CVE list for YAML deserialization CVEs to find the correct CVE.

Flag: CTF{CVE-2022-1471}


## 8. Lunar Light
<img width="906" alt="image" src="https://github.com/user-attachments/assets/b0e7e388-8a33-4d26-ac2f-eb4d65aca376" />
<img width="582" alt="image" src="https://github.com/user-attachments/assets/a3c9acde-8969-4d4f-a008-960210ff6b8b" />

Method: I opened the image in an image editor then manipulated the exposure and other settings to see the flag.

Flag: CTF{M00NLIT_R3V3AL}


## 9. Paths to Prosperity
<img width="463" alt="image" src="https://github.com/user-attachments/assets/836b7a1d-e43d-424e-8be4-e48c3df5b9ae" />
<img width="1292" alt="image" src="https://github.com/user-attachments/assets/37175295-04a6-4a49-99e1-efe8873f7c90" />

Method: Using the developer tools I was able to see hidden directories in the sources for the webpage to find the page containing the flag.  then used JavaScript injection to obtain the flag.

Flag: CTF{traversing_new_paths}


## 10. Python's Passwords
<img width="952" alt="image" src="https://github.com/user-attachments/assets/1f57774d-1325-42bc-999b-0c1bb5d937c6" />

Method:

Flag:


## 11. Snake
<img width="495" alt="image" src="https://github.com/user-attachments/assets/45a8e8c0-2aef-4aef-b179-ca24c7e968fd" />

Method:

Flag:
