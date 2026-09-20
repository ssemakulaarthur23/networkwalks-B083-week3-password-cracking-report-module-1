# networkwalks-B083-week3-Password Cracking with John the Ripper (JTR) & Johnny

## Objective
Use John the Ripper (JTR) and Johnny GUI to recover the password of a protected PDF file on Windows.  
This lab demonstrates how password cracking works and why strong passwords are important. All evidence of this project is in the screenshots above

## Tools Used
- John the Ripper (JTR) – https://www.openwall.com/john/
- Johnny GUI – https://openwall.info/wiki/john/johnny
- OnlineHashCrack PDF Hash Extractor – https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php
- Windows PC
- Lab file: `My Locked PDF1.pdf`

> Note: If you are using Kali Linux, John the Ripper comes pre-installed and can be opened directly.

## Ethical Disclaimer
This project is for educational purposes only.  
All testing was performed on a lab file I own or have permission to test.  
Do not use these techniques on systems or files you do not own or have explicit permission to test.

## Lab Environment
- OS: Windows
- Tools: John the Ripper, Johnny GUI
- Target: `My Locked PDF1.pdf`
- Hash file: `hash1.txt`

## Lab Steps

### 1. Download and Install John the Ripper
Downloaded JTR from the official Openwall website and installed it on Windows.

### 2. Download and Install Johnny GUI
Downloaded Johnny 2.2 from the official Openwall wiki and ran `johnnyInstaller.exe`.

### 3. Configure Johnny
Opened Johnny → **Settings** → **Browse** → selected the John the Ripper executable path.

### 4. Extract the PDF Hash
Used OnlineHashCrack PDF Hash Extractor:
- Uploaded `My Locked PDF1.pdf`
- Copied the generated hash
- Removed extra characters like `b'` at the start if present
- Saved the hash as `hash1.txt`

Example hash format:
```text
$pdf$4*4*128*-1060*1*16*...*32*...
