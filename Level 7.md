# Level 7 Solution

**The password for the next level is stored in the file data.txt next to the word millionth.**

## Login
```bash
ssh -p 2220 bandit7@bandit.labs.overthewire.org
```

## Password
```bash
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```

## 1. Using grep
```bash
cat data.txt | grep "millionth*"
```
It will find the word millionth and give the password next to it.

## 2. Using VIM Editor
```bash
vim data.txt
```
This will open the file in vim editor.
Here we can search the word "millionth" by using "?".
As soon as we type "?" we will enter find mode and can search inside that file.
