# Level 9 Solution

**The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.**

## Login
```bash
ssh -p 2220 bandit9@bandit.labs.overthewire.org
```

## Password
```bash
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```

## 1. Use VIM Editor
```bash
vim data.txt
```
Search for multiple "=" using ?.

## 2. Strings Method
```bash
strings data.txt
```
It will give only human readable strings.

**Combine it with grep**
```bash
strings data.txt | grep "="
```
