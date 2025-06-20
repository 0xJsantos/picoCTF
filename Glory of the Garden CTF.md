# CTF Writeup: Glory of the Garden

**Author:** John Bless Santos  
**Challenge Name:** Glory of the Garden  
**Category:** Forensics  
**Platform:** picoCTF  
**Flag:** picoCTF{more_than_m33ts_the_3y33dd2eEF5}

## Overview

We were given a file called `garden.png` and a hint to use a hex editor. Our goal was to find a hidden flag in the file.

## Tools Used

- xxd – to create a hex dump
- cat and grep – to search through the file
- gedit – to open and view the dump file
- Ctrl + F – to search for keywords in gedit

## Steps

1. **Download the File**  
   We downloaded the file `garden.png`.
   
   ![Image](https://github.com/user-attachments/assets/e0c42a25-a858-4ace-b3b6-09d88ca11f69)

3. **Check the Hint**  
   The challenge hint said to use a hex editor, which shows the file’s raw data and ASCII content.

4. **Make a Hex Dump**  
   We used this command to turn the image into a readable format:
   
   ![Image](https://github.com/user-attachments/assets/b8112054-594b-4543-822e-64de8e7de6b7)

6. **Try Searching Automatically**  
   We ran this command to look for the flag:
  It didn’t work, so we moved to manual inspection.

7. **Open and Search Manually**  
  We opened the file in gedit:
  Then we used Ctrl + F to search for words like `pico`, `flag`, and `ctf`.

8. **Find the Flag**  
  After scrolling and searching, we found the flag in the ASCII part of the file.
   ![Image](https://github.com/user-attachments/assets/165bec15-b620-4fdb-8105-519f5dcfaf92)

## Flag
  picoCTF{more_than_m33ts_the_3y33dd2eEF5}



