# To login Level 3

**The password for the next level is stored in a file called --spaces in this filename-- located in the home directory**

## Login in level 2:
```bash
ssh -p 2220 bandit2@bandit.labs.overthewire.org
```
## Password:
```bash
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```

### There are differrent ways to read a file with spaces in its name:

**Use * if the file is unique**
```bash
cat ./--spaces*
```
With this we can skip all the spaces.

**Use \ before every space**
```bash
cat ./--spaces\ in\ this\ filename--
```
