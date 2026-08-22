# OverTheWire Bandit 

## Level 0 → 1
Logged into bandit0 via SSH. Used `cat readme` in the home directory to find the password for bandit1.

## Level 1 → 2
Password was stored in a file literally named `-` (a dash). Learned that `cat -` gets interpreted as reading from stdin instead of the file, so you have to reference it differently `cat ./-` to read a file named `-`.

## Level 2 → 3
Filename contained a space. Learned to either wrap the filename in quotes or escape the space with a backslash so the shell treats it as one filename instead of two arguments.

## Level 3 → 4
File was hidden inside the `inhere` directory. A plain `ls` showed nothing, but `ls -la` revealed a file named `...Hiding-From-You`. We can also use the command `find`.
