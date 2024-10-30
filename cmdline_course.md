## Command line for linquistics course KIK-LG219


_This page includes:_

[The course syllabus](#the-course-syllabus)

[My notes](#my-notes)

[Usefull links](#usefull-links)

[Handy video tutorials](#handy-video-tutorials)

--- 

### The course syllabus

**Week 1: Introduction to Command-Line Linux**

Main topics:
* How to install and use Windos subsystem for Windows
* Using command-line basic commands
* Using text editors in command line (Nano)
* File formats (pdf, doc, jpeg, png, mp4)

First weeks main thing is to get the command line up and running regardless of what OS they are using. I am a Windows user, so I am using Linux subsystem for Linux. After completing that the next task is to learn how to navigate in command line environment: creating and deleting files and folders, moving between folders, how to open a file to read (Nano). 

_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `ls` | Lists files and directories. |
| `pwd` | Prints the current working directory. |
| `whoami` | Prints the users username |
| `cd` | Changes the current directory. |
| `nano` | Simple text editor for command line. |
| `wget` | Download files from the internet. |
| `mv` | Moves or renames files and directories. |
| `cat` | Displays the contents of a file. |
| `less` | Views the contents of a file one page at a time.|
| `cp` | Copies files or directories. |
| `rm` | Removes files or directories. |
| `mkdir` | Creates a new directory. |
| `cd` | Changes the current directory. |
| `cd ..` | Moves up one directory level. |

---

**Week 2: Navigating a UNIX System**

Main topics:
* The UNIX filesystem
* Commands
* Users, groups and file permissions
* Working in a remote server

The second week of this course included more navigating in the UNIX environment from the command line. Also connected to a remote system using SSH (secure shell protocol).

_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `cp -R` | Recursively copies directories and their contents. |
| `rm -R` | Recursively removes directories and their contents. |
| `rmdir` | Removes empty directories. |
| `which` | Shows the full path of shell commands. |
| `top` | Displays real-time system processes and resource usage. |
| `&` | Runs a command in the background. |
| `fg` | Brings a background job to the foreground. |
| `CTRL+Z` | Pauses a foreground job, sending it to the background. |
| `ps` | Lists currently running processes. |
| `kill` | Terminates a process by its ID. |
| `ssh` | Connects to a remote system via SSH. |
| `scp` | Securely copies files to or from a remote system. |

---

**Week 3: Corpus Processing**

Main topics:
* Processing text files 
* Processing data files
* Regular expressions introduction

The third week is about text and data file processing. 

_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `file` | Determines the type of a file. |
| `dos2unix` | Converts Windows line endings to Unix format. |
| `iconv` | Converts text from one encoding to another. |
| `tr` | Translates or deletes characters from input. |
| `sort` | Sorts lines of text files. |
| `uniq` | Removes duplicate lines from sorted input. |
| `egrep` | Searches for patterns using extended regular expressions. |
| `cut` | Extracts sections from each line of a file. |
| `sort` | Sorts lines of text files (included for completeness). |
| `uniq` | Removes duplicate lines (included for completeness). |
| `egrep -w -f` | Searches for exact word matches in patterns from a file. |

---

**Week 4: Scripting and Version Control**

Main topics:
* Searching (grep)
* Editing files (sed) 
* Combining commands into a script

Week 4 is about the basics of scripting, with a focus on combining multiple commands into reusable scripts. Tools like `grep` and `sed` can be used for advanced searching and editing, improving text filtering and modification skills (and this required lots of learning from mistakes, e.g. not easy week for me). 

_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `grep` | Searches text using patterns. |
| `sed` | Edits text in a scriptable way. |
| `sed -n` | Suppresses automatic printing of pattern space (useful for selective printing). |
| `sed -E` | Enables extended regular expressions in `sed`. |
| `sed '/pattern/d'` | Deletes lines that match the specified pattern. |
| `sed -n '/pattern/p'` | Prints only lines that match the specified pattern. |
| `sed 's/pattern/replacement/g'` | Replaces all occurrences of a pattern in each line. |

---

**Week 5: A Deeper Look at the UNIX System**

Main topics:
* Environment variables
* Configuration files (.bashrc, .bash_history, .bash_profile)
* Writing own scripts

Week 5 is about configuration files, environment variables, and custom script creation. More learning from mistakes.


_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `chmod u+x` | Grants execute permission to the user for a file. |
| `if` | Starts a conditional statement in shell scripts. |
| `$?` | Returns the exit status of the last command. |
| `$#` | Shows the number of positional parameters passed to a script. |
| `printenv` | Displays environment variables. |
| `echo` | Outputs text or variable values to the terminal. |
| `export` | Sets an environment variable for the current session. |
| `~/.bashrc` | Initialization file executed for interactive shells. |
| `~/.bash_profile` | Initialization file for login shells (on some systems). |
| `source` | Executes commands from a file in the current shell. |
| `alias` | Creates or lists command shortcuts. |

---

**Week 6: Installing and Running Programs**

Main topics:
* Root user
* Installing and running python-based software
* Creating your virtual environments
* Building projects using Make 

This week we learned from different user levels (thou must be careful to use sudo!). Also learned about packet managers for installing packages. Makefiles help automate larger projects and after spending two hours of trying to fix your makefile logic only to find out a TYPO you really need a break.


_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `sudo` | Runs a command with superuser privileges. |
| `su` | Switches to another user account. |
| `whoami` | Displays the current user's username. |
| `passwd` | Changes the password for a user account. |
| `apt-get` | Installs, updates, or removes packages on Debian-based systems. |
| `brew` | Installs and manages packages on macOS systems. |
| `locate` | Finds files by name on the system. |
| `python` | Runs the Python interpreter. |
| `pip` | Installs and manages Python packages. |
| `pip install` | Installs a specified Python package. |
| `pip install --user` | Installs a Python package for the current user only. |
| `make` | Builds and manages projects using Makefiles. |
| `make all` | Builds all targets specified in a Makefile. |
| `make clean` | Removes files generated by the build process. |

---

**Week 7: Version control**

Main topics:
* Git & Github
* Setting up Git repository
* Committing changes
* Git branches

<img src="https://cdn.masto.host/socialjvnsca/media_attachments/files/111/902/671/570/742/924/original/6198af3309e7e932.png" alt="https://social.jvns.ca/@b0rk/111902671879692064" widt="30%" align=center">

There is a reason why XKCD makes so many jokes of Git and version control. This weeks topics were about setting up a very own github remote repository, how to commit changes and have branches for different functionalities/parts. (Gues how many times I restarted my git page because I didn’t read the instructions properly? Its more than two.)



_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `git init` | Initializes a new Git repository. |
| `git add` | Stages changes for the next commit. |
| `git commit` | Commits staged changes with a message. |
| `git branch` | Manages branches within a repository. |

---

**Final project**
Main topics:
* Building Webpages using GitHub Pages

Github pages were a new feature for me but a very useful. I spent hours on building my project and a lot of time was spent to waiting for the changes to be updated on server. 


_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `git push` | Pushes commits to a remote repository. |
| `git clone` | Clones a repository to your local machine. |
| `gh-pages` | Deploys to GitHub Pages (usually via plugin). |
| `jekyll` | Builds static sites for GitHub Pages. |
| `bundle install` | Installs depencies. |
| `bundle exec jekyll serve` | Run jekyll to build a local site. |

---

### My notes

[Nano cheat sheet](https://katja-cmd.github.io//nano_cheat_cheet.html)

[Command line cheat sheet](https://katja-cmd.github.io/cmd_line_cheat_sheet.html)

[Git cheat sheet](https://katja-cmd.github.io/git_cheat_sheet.html)

[Git markdown cheat sheet](https://katja-cmd.github.io/github_markdown_cheat_sheet.html)

### Usefull links

[Komentorivityökalut (FI)](https://tim.jyu.fi/view/kurssit/tie/ohj1/tyokalut/komentorivi)

[UNIX Tutorial](https://people.ischool.berkeley.edu/~kevin/unix-tutorial/toc.html)

[GitHub Pages tutorial](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages)

[Git ja Github: versionhallinta (FI)](https://tkt-lapio.github.io/git/)

[GitHub Student Developer Pack](https://education.github.com/pack)

[Regular Expressions Cheat Sheet](https://cheatography.com/davechild/cheat-sheets/regular-expressions/)

[CSV file tutorial](https://www.computerhope.com/issues/ch001356.htm)

[Sed tutorial](https://www.grymoire.com/Unix/Sed.html)

[Regular expressions tutorial](https://www.regular-expressions.info/tutorial.html)

[Script tutorial](https://ryanstutorials.net/bash-scripting-tutorial/bash-script.php)

[The Difference Between su and sudo Commands In Linux](https://www.rootusers.com/the-difference-between-su-and-sudo-commands-in-linux/)

[What is a Makefile and how does it work](https://opensource.com/article/18/8/what-how-makefile)


### Handy video tutorials

[How to Run Linux/Bash on Windows 10 Using the Built-In Windows Subsystem for Linux](https://youtu.be/xzgwDbe7foQ?si=n5Cxxd-OAT3T4TKP)

[Git Tutorial for Beginners: Command-Line Fundamentals](https://youtu.be/HVsySz-h9r4?si=DlZWv3Vi5mVwW3zG)

[Git Tutorial: Fixing Common Mistakes and Undoing Bad Commits](https://youtu.be/FdZecVxzJbk?si=wb5NKBNszdHYQh3I)

[Git Tutorial: Difference between "add -A", "add -u", "add .", and "add *"](https://youtu.be/tcd4txbTtAY?si=MhbT2GI31uIpNyZh)

[Command line crash course for beginners](https://www.youtube.com/watch?v=uwAqEzhyjtw&pp=ygUVY29tbWFuZCBsaW5lIHR1dG9yaWFs)

[Markdown crash course](https://youtu.be/_PPWWRV6gbA?si=xkhRn7HxPO1NEHXn)

[Linux directories explained](https://youtu.be/42iQKuQodW4?si=l4GvLeo8rmUVioXB)

[Bash in 100 seconds](https://youtu.be/I4EWvMFj37g?si=sq5UzteERIxRnBYR)



