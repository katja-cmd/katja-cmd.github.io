## Command line for linquistics course KIK-LG219

This course introduces the basics of command-line tools with a linquistics focus. It starts from the basics – no prerequisites needed! (But if you have any experience in programming, it will be useful.) The first week starts from basic navigation and file handling, introduces regular expressions and script writing, and end with publishing a web page via Github pages using branching and version control tools. 


_This page includes:_

[The course contents](#the-course-contents)

[My notes (e.g. collection of cheat sheets)](#my-notes)

[Useful links to written tutorials](#usefull-links)

[Handy video tutorials](#handy-video-tutorials)

--- 

### The course contents

**Week 1: Introduction to Command-Line Linux**

Main topics:
* How to install and use Windos subsystem for Windows
* Using command line basic commands
* Using text editors in command line (Nano)
* File formats (pdf, doc, jpeg, png, mp4)

First weeks main thing is to get the command line up and running regardless of what ever OS anyone are using. I am a Windows user, so I am using Linux subsystem for Linux. Not as easy as one would think. After completing that the next task was to learn how to navigate in command line environment: creating and deleting files and folders, moving between folders, how to open a file to read in a program (Nano) or just display the file contents in command line (cat). We also learned how to download a text files from internet and search key words from it. Important to remember: with tab key we can get previously used command from memory and tje general copy and paste keyboard shortcuts are not the same as in Windows (ctrl+C -> Ctrl+Shitf+C).

_Example code snippet of this week:_

```
$ wget [URL] 
```
This command downloads content from the given url.

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

The second week of this course included more navigating in the UNIX environment from the command line like copying files to another folders, creatings links to files, and how to remove folders when there is or is not contents. Also learned how to connect to a remote system using [SSH (secure shell protocol)](https://en.wikipedia.org/wiki/Secure_Shell). (Be aware: after getting the connection to Puhti working, the spam emails cannot be stopped.)


_Example code snippet of this week:_

```
$ killall <process_name>
```
This command kills a named process.


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

The third week is about text and data file processing. We learned how to remove line breaks from a .txt file, re-arranging lines in a text file (usefull maybe in a word lists?), searching patters (grep), and checking how many lines a .txt file has (note to self: in Nano the show line numbers command is Alt-C). We alse learned to create word frequency lists with a really long one line command that are very prone to typos (and that's why we create scripts).


_Example code snippet of this week:_

```
$ cat book.txt  2> errors.txt| tr '\n' ' ' > output.txt
```
This command transforms book.txt into one long line and prints potential error messages from cat to errors.txt. The output from the tr command is directed to output.txt.

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

Week 4 is about the basics of scripting, focusing on combining multiple commands into handy scripts. Commands like `grep` and `sed` can be used for advanced searching and editing, improving text filtering and modification skills (and this required lots of learning from mistakes, e.g. not easy week for me -  needed to have emergency chocolate next to me when doing this weeks homework). We also learned to create n-grams from a .txt file.


_Example code snippet of this week:_

```
$ cat life_of_bee.txt | tr -s '\n\r\t ' '\n' | tr -dc "A-Za-z0-9'\n" | egrep "^[A-Z]" | wc -l
```
This pipeline code takes life_of_bee.txt file, transforms it into a one word per line format, removes punctuations and finally outputs the contents with 'cat'. TThe output is count of the number of lines in life_of_bee.txt that start with an uppercase letter after all the cleaning.


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

Week 5 is about configuration files, environment variables, and custom script creation. More learning from my own mistakes. After creating a script I need to give permission to execute it before running it and isn't that fun thing to realize after debugging the script for three hours. Another mistake I made recursively was to not include the script path when trying to execute it from a different folder. 


_Example code snippet of this week:_

```
#!/bin/bash
echo "$1er"
```
This code is a bash script that takes one argument (an English adjective) and prints its comparative form ending "-er". 


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

This week we learned from different user levels (thou ought to be careful when using sudo!). Also learned about packet managers for installing packages (pip). Makefiles help automate larger projects and after spending two hours of trying to fix your makefile logic only to find out a TYPO you really need a break. 


_Example code snippet of this week:_

```
$ pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```
This command uses pip to install the Deep Learning library of Python, called Pytorch.


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

<img src="https://cdn.masto.host/socialjvnsca/media_attachments/files/111/902/671/570/742/924/original/6198af3309e7e932.png" alt="https://social.jvns.ca/@b0rk/111902671879692064" width="70%" style="display: block; margin: 0 auto;">


There is a reason why XKCD makes so many jokes of Git and version control. This weeks topics were about setting up a very own github remote repository, how to commit changes and have branches for different functionalities/parts. (Gues how many times I restarted my git page because I didn’t read the instructions properly? Its more than two.) The branching functionality makes sense in a bigger projects with more than one contributor, but I don't really see the point to use several branches when working by myself.


_Example code snippet of this week:_

```
$ git config --global user.name "Aku Ankka"
$ git config --global user.email "aku@ankkalinna.com"
```
These commands set user.name and user.email to git.


_New commands I learned this week:_

| Command | Description |
|---------|-------------|
| `git init` | Initializes a new Git repository. |
| `git add` | Stages changes for the next commit. |
| `git commit` | Commits staged changes with a message. |
| `git branch` | Manages branches within a repository. |

---

**The Final project**

Main topics:
* Building Webpages using GitHub Pages
* Using Jekyll templates
* LateX

Github pages were a new feature for me but a very useful. I spent hours on building my project and a lot of time was spent to waiting for the changes to be updated on server. We learned to use LateX to make cv from a template. I have used LateX briefly before and we are not in speaking terms. Minor changes could make everything collaps and I learned to hit "compile" every 10 seconds to find my errors before writing something in lenght only to realize it don't work. Microsoft Office is not perfect, but I think I will stick with it and deal with bugs rather than use LateX.


_Example code snippet of this week:_

```
$ git add .
$ git commit -m "Typo corrections, again (I might be dyslexic)"
$ git push
```
These commands add all modifield files to commit, does the Git commit with a dsescribing comment (that should actually be a bit more formal) and pushes the changes to remote repository.


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

<img src="/assets/images/gitlogo.png" alt="XKCD comic about Git" hspace="20" width="15%" align="center"/>


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



