# CTF Writeup: Information

**Author:** John Bless Santos  
**Challenge Name:** Information  
**Category:** Forensics  
**Platform:** picoCTF  

## Overview

We were given a file called `cat.jpg` and three hints:

- Look at the details of the file  
- Make sure to submit the flag as picoCTF{XXXXX}  
- Files can be changed in a secret way

These hints suggested that steganography or metadata analysis would be needed to find the hidden flag.

## Tools Used

- xxd – to make a hex dump of the image  
- grep – to search for strings  
- exiftool – to view file metadata  
- base64 – to decode any hidden strings  

## Steps

1. **Download the File**  
   We started by downloading `cat.jpg`.

2. **Hex Dump Inspection**  
   We created a hex dump of the image:
xxd cat.jpg > catdump.txt

   Then we used `grep` to try to find the flag:

