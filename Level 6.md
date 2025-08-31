**The password for the next level is stored somewhere on the server and has all of the following properties:**
- **owned by user bandit7**
- **owned by group bandit6**
- **33 bytes in size**
# Level 6 Solution:

## Login
```bash
ssh -p 2220 bandit6@bandit.labs.overthewire.org
```

## Password
```bash
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```

## Run:
```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
```

- **find /** will start finding from home directory because it can be anywhere.
- **-type f** will find only files.
- **-user username** will find the files owned by that specific user.
- **-group groupname** will find the file belonging to that group.
- **-size 33c** returns the file only with size of 33 bytes.
- **2>** will redirect all the error messages like "Permission Denied"" to null folder.
- **/dev/null** nullifies every thing redirected to it, like a black hole.

## I/O Redirection:
This is a process to redirect the standard input or output to a desired file.
For Example: We executed a command, let's take the ls command, and instead of showing its result want to write in a file we can do it.
There are specific codes for that.
- **0** for standard input.
  Example: We have written a code which requires manual input, we can redirect it to a file that will take its input from that file.
  ```bash
  wc -l < file.txt
  ```
  Word count will take input from file.txt
- **1** for standard output.
Example: ls >list.txt

- **2** for standard error.
As discussed above.
