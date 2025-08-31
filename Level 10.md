# Level 10 Solution

**The password for the next level is stored in the file data.txt, which contains base64 encoded data.**

## Login
```bash
ssh -p 2220 bandit10@bandit.labs.overthewire.org
```

## Password
```bash
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```

## Run
```bash
base64 -d data.txt
```
**Base64** is a encrypting method which is used to hide the original content of a file. Its **options are**
- **-e** Encode
- **-d** Decode
- **-i** Ignore non encoded lines
