# Solving Level 4

**The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.**

## Login
```bash
ssh -p 2220 bandit4@bandit.labs.overthewire.org
```

## Password
```bash
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```
 **Ways to find the password of next level**
 -Check all the files.
 -Use command to find the content type of file:
 ```bash
file ./*
```
Whichever file contains **ASCII Text** or **UTF-8 Text** is humand readable. 
