# 🔒 Password Hash Cracking using John the Ripper & Hashcat

This project was completed as part of my **Cybersecurity Analyst course provided by IBM**.  
It demonstrates how SHA-512 password hashes can be cracked using dictionary attacks with **John the Ripper** and **Hashcat** on a Windows system.

---

## 🛠️ Tools Used
- John the Ripper (Jumbo build for Windows)
- Hashcat v6.2.6
- Wordlist: `listofpasswords.txt`
- Hash Type: SHA-512 (`-m 1700`)
- Operating System: Windows 10

---
## 💻 Commands Used

### 🔹 John the Ripper:
john --format=raw-sha512 --wordlist=wordlists\listofpasswords.txt hashes.txt

### 🔹 HashCat:
hashcat.exe -m 1700 -a 0 --username hashes.txt wordlists\listofpasswords.txt

⚠️ Disclaimer
This project is for educational purposes only.
All passwords and hashes used were self-generated in a controlled lab environment.
No real systems or credentials were used or compromised.
