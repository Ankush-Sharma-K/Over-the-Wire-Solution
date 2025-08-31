# Solving Level 5:

**The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:**
- **human-readable**
- **1033 bytes in size**
- **not executable**

## Login
```bash
ssh -p 2220 bandit5@bandit.labs.overthewire.org
```

## Password
```bash
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```

## Run
```bash
find /path/to/directory -type f -size 1033c ! -executable -exec file {} \; | grep "text"
```
**Or you can run just if you are inside that directory**
```bash
find -type f -size 1033c ! -executable -exec file {} \; | grep "text"
```

### find:
This is used to find the files or directories inside a directory.
This is real time based command, it searches for the file in real time unlike **locate**.
We can talk about the differnce between locate and find in my **Interview Questions** Directory.

### -type f:
This defines that we need result from types of files if this is not specified then it will go for the directories also.

### -size 1033c
This will search for the files of size 1033 bytes.
- c goes for bytes
- k for kilobytes
- m for megabytes
- g for gigabytes
- b for 512 bytes block
- w for 2 bytes

  ### !:
  Denotes the logical **NOT**

  ### -executable:
  Means the file is executable.

  ### -exec:
  if we want to run another command on the result we got we use this.

  ### file:
  it is a command that shows the type of files.

  ### {}:
  Well it is just a holder it will be placeholder and will be replaced by the current filename.

  ### \;
  - ; is for ending the exec command.
  - \ is an escaping character.

  ### |
  This means that the outut of left command will be input for right command.

  ### grep:
  Searches for text or patterns and shows the result only that contains that result.
