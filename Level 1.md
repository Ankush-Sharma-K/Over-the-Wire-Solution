# To reach Level 2:

**The password for the next level is stored in a file called - located in the home directory**

The files name starting with **-** are really annoying beacause as we go to perform any actons like cat or any other file operations
the terminal will understand the text after **-** as a command option, and throw an error.
**To tackle this we can use ./ before the filename.**

## Login in the level 1.
```bash
ssh -p 2220 bandit1@bandit.labs.overthewire.org
```

## Password
```bash
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```

**Read the file for password**
```bash
cat ./-
```
