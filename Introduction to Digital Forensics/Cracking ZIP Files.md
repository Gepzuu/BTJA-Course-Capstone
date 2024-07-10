# Activity:
<div align="justify">
BruteForceAttack.zip – You are to brute-force this ZIP file using fcrackzip. Once you have the password, extract the text file FLAG1.txt and enter the text string as your answer for the quiz. For this file, you have been informed that the password is 6 characters long, and contains only lowercase letters, and numbers. <br><br>
DictionaryAttack.zip – You are to brute-force this ZIP file using fcrackzip and the rockyou.txt wordlist. Once you have the password, extract the text file FLAG2.txt and enter the text string as your answer for the quiz. <br><br>
</div>

## Tools Used:
Linux<br>
fcrackzip

## Questions:
1. What is the working password to unlock BruteForceAttack.zip?<br>
2. What is the working password to unlock DictionaryAttack.zip?<br>
3. What is the text string inside FLAG1.txt? <br>
4. What is the text string inside FLAG2.txt? <br><br>

## Answers:
1. a1b3c5 <br>
2. FRIENDSHIPSTARS <br>
3. J201AKKLO <br>
4. 91MD0QL11 <br><br>

In this activity, the Security Blue Team gave me a zip file to crack. <br>
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/0aa03441-bf62-42d8-8f5c-a6a16a385403">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/39ca45a6-8d4b-4c4c-8837-7598b93de684">
</div><br><br>

Install fcrackzip <br>
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/b27571c9-f250-42b5-b614-6a4e6eaad0e9">
</div><br><br>

The command to crack the zip file BruteForceAttack.zip is 'fcrackzip -D -u -p /usr/share/wordlists/rockyou.txt BruteForceAttack.zip'. <br><br>
-D: This option tells fcrackzip to use a dictionary attack, which means it will try to crack the password by trying a list of words from a file. <br><br>
-u: This option tells fcrackzip to try to crack the password using uppercase and lowercase letters. <br><br>
-p: This option specifies the path to the dictionary file that fcrackzip will use to try to crack the password. <br><br>

When you run this command, fcrackzip will try to crack the ZIP file's password using the words in the rockyou.txt dictionary file. <br> <br>

The command reveals the password to be 'a1b3c5'. <br>
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/2653c3e4-127e-4b19-ae79-6477bf4b2b0e">
</div><br><br>

I used the password 'a1b3c5' to unzip a file called 'BruteForceAttack.zip.' Upon unzipping it, I discovered a secret code inside: 'J201AKKLO'. <br><br>

I used fcrackzip to crack the 'DictionaryAttack.zip' file, repeating the previous process. <br><br>
<div align="center">
<img src=https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/29ffab59-27e3-44d0-8924-4c985b344fbe">
</div><br><br>

After typing the command, the password was found to be 'FRIENDSHIPSTARS'. <br>
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/2653c3e4-127e-4b19-ae79-6477bf4b2b0e">
</div><br><br>

Using the password 'FRIENDSHIPSTARS', I unzipped the 'DictionaryAttack.zip' file and found a secret code inside: '91MD0QL11'. <br><br>



