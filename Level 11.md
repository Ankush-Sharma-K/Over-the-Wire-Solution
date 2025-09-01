# Level 11 Solution

**The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions.**

## Login
```bash
ssh -p 2220 bandit11@bandit.labs.overthewire.org
```

## Password
```bash
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```

## Run
```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```
- **tr** Stands for translate.
```bash
tr [OPTION] SET1 [SET2]
```
- **Set1** Characters you want to match.
- **Set2** Characters you want them to become.

**Example**
```bash
echo 'ram ram' | tr 'a-z' 'A-Z'
```
```
RAM RAM
```
### Its Options are:
- **-d** Deletes the charaters.
```bash
tr -d '0-9'
```

- **-s** Squeeze Repeated Characters.
- **-cd** Replace all except the given set.
