## Command line commands - my cheat sheet

## General file and directory management commands

| Command | Description |
|---------|-------------|
| `cat` | Displays the contents of a file. |
| `cd` | Changes the current directory. |
| `cd ..` | Moves up one directory level. |
| `cp` | Copies files or directories. |
| `cp -R` | Recursively copies directories and their contents.|
| `mkdir` | Creates a new directory. |
| `mv` | Moves or renames files and directories. |
| `pwd` | Prints the current working directory. |
| `rm` | Removes files or directories. |
| `rm -R` | Recursively removes directories and their contents.|
| `rmdir` | Removes empty directories. |
| `touch` | Creates an empty file. |

---

### Text processing commands

| Command | Description |
|---------|-------------|
| `cut` | Extracts sections from each line of a file. |
| `dos2unix` | Converts Windows line endings to Unix format. |
| `egrep` | Searches for patterns using extended regular expressions. |
| `egrep -w -f` | Searches for exact word matches in patterns from a file. |
| `grep` | Searches text using patterns. |
| `iconv` | Converts text from one encoding to another. |
| `less` | Views the contents of a file one page at a time. |
| `sort` | Sorts lines of text files. |
| `tr` | Translates or deletes characters from input. |
| `uniq` | Removes duplicate lines from sorted input. |
| `nano` | Simple text editor for command line. |
| `sed` | Edits text in a scriptable way. |
| `sed -E` | Enables extended regular expressions in `sed`. |
| `sed -n` | Suppresses automatic printing of pattern space. |
| `sed '/pattern/d'`| Deletes lines that match the specified pattern. |
| `sed -n '/pattern/p'`| Prints only lines that match the specified pattern. |
| `sed 's/pattern/replacement/g'`| Replaces all occurrences of a pattern in each line.|

--- 

### Permission and user management commands

| Command | Description |
|---------|-------------|
| `alias` | Creates or lists command shortcuts. |
| `chmod` | Changes file permissions. |
| `chmod u+x` | Grants execute permission to the user for a file. |
| `chown` | Changes file owner and group. |
| `passwd` | Changes the password for a user account. |
| `sudo` | Executes a command with superuser privileges. |
| `su` | Switches to another user account. |

---

### Other commands

| Command | Description |
|---------|-------------|
| `apt-get` | Installs, updates, or removes packages. |
| `brew` | Installs and manages packages on macOS systems. |
| `clear` | Clears the terminal screen. |
| `CTRL+Z` | Pauses a foreground job, sending it to the background. |
| `df` | Displays disk space usage. |
| `du` | Displays directory space usage. |
| `echo` | Outputs text or variable values to the terminal. |
| `exit` | Closes the terminal session. |
| `fg` | Brings a background job to the foreground. |
| `history` | Shows command history. |
| `kill` | Terminates a process by its ID. |
| `man` | Shows manual for a command. |
| `pip` | Installs and manages Python packages. |
| `pip install` | Installs a specified Python package. |
| `pip install --user` | Installs a Python package for the current user only. |
| `printenv` | Displays environment variables. |
| `ps` | Lists currently running processes. |
| `scp` | Securely copies files to or from a remote system. |
| `ssh` | Connects to a remote system via SSH. |
| `source` | Executes commands from a file in the current shell.|
| `top` | Displays real-time system processes and resource usage.|
| `wget` | Downloads files from the internet. |
| `whoami` | Prints the user's username. |
| `~/.bashrc` | Initialization file executed for interactive shells.|
| `~/.bash_profile` | Initialization file for login shells (on some systems). |
| `&` | Runs a command in the background. |

