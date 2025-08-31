# Level 8 Solution

**The password for the next level is stored in the file data.txt and is the only line of text that occurs only once.**

## Login
```bash
ssh -p 2220 bandit8@bandit.labs.overthewire.org
```

## Password
```bash
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```

## Run
```bash
sort data.txt | uniq -u
```

- **sort** Sorts the file. It is necessary because uniq command runs only on a sorted file.
- **uniq** gives the result according to the option
- **-u** prints only the unique line.
- **-c** count each line.
- **-d** Shows only duplicate, once each.
