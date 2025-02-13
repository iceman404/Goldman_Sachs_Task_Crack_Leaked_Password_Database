## Goldman_Sachs_Task_Crack_Leaked_Password_Database

**Since the leaked password are all 32 characters long, that means these are MD5 Hashes, 
So we try to crack these MD5 Hashes using Hashcat or John the Ripper.**

## 1. Install Hashcat or John the Ripper:
```bash
sudo apt-get update
sudo apt-get install hashcat
```

## 2. For John the Ripper:
```bash
sudo apt-get update
sudo apt-get install john
```

## To use Hashcat, we can use the -m 0 flag (MD5 mode) in Hashcat.
```bash
hashcat -m 0 -a 0 password_dump.txt ./wordlist.txt
```

## For John the Ripper we can use:
```bash
john --format=raw-md5 password_dump.txt
```
## We can use a popular wordlist, like the rockyou wordlist, which can be found online.

**Wordlist: Both tools work best with a large wordlist of potential passwords. We can download rockyou.txt or any other popular wordlist from public repositories or use a wordlist of your own.**

## Monitor Progress:

**Both tools will output the cracked passwords in the terminal once they find a match. For Hashcat, we can monitor progress using:**
```bash
hashcat -m 0 -a 0 --status hashes.txt ./wordlist.txt
```

## Performance Considerations:
**Cracking passwords using GPU acceleration with Hashcat would be much faster on a local machine with powerful hardware, However we can still crack MD5 hashes if we're using CPU-based cracking or moderate-sized wordlists.**

## Limitations:
**Speed: The cracking speed will likely be slower than using dedicated hardware or a GPU setup.**



