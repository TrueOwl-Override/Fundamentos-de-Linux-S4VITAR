<div align="center">

# 🐧 Fundamentos de Linux · S4VITAR

**My notes from S4vitar's Linux fundamentals course: Linux commands and Bash scripting, grouped by what they do, with copy-ready examples.**

![Commands](https://img.shields.io/badge/commands-137-2ea44f?style=for-the-badge) ![Parameters](https://img.shields.io/badge/parameters-167-0969da?style=for-the-badge) ![Categories](https://img.shields.io/badge/categories-23-8250df?style=for-the-badge)

🌐 **Searchable web version:** [`docs/index.html`](docs/index.html)

</div>

---

## 📚 Categories

### 🐧 Linux Commands

| | Category | What's inside | Commands |
|:-:|:--|:--|:--|
| 📁 | **[Navigation & Files](notes/navigation-files.md)** | Move around the filesystem and create, copy, delete and inspect files and folders. | `pwd` `ls` `cd` `mkdir` `touch` `cp` `rm` `file` `stat` `*` |
| 📝 | **[Viewing & Editing Files](notes/viewing-editing-files.md)** | Read files in the terminal, page through output, compare files and edit text. | `cat` `more` `head` `tail` `rev` `diff` `nano` `vi` |
| 🔍 | **[Searching](notes/searching.md)** | Find files anywhere on the system and locate where commands live. | `find` `grep` `which` `command` `xargs` |
| ✂️ | **[Text Processing](notes/text-processing.md)** | Filter, cut, transform and sort text coming from files or other commands. | `echo` `awk` `cut` `tr` `sed` `sort` `uniq` `tee` `sponge` `column` |
| 🔀 | **[Pipes, Redirection & Operators](notes/pipes-redirection-operators.md)** | Chain commands, decide where output and errors go, and run things in the background. | `\|` `;` `&&` `\|\|` `&` `>` `>>` `2>/dev/null` `2>&1` `&>/dev/null` `exec` `disown` |
| 👤 | **[Users & Groups](notes/users-groups.md)** | Check who you are, switch users, and manage accounts, passwords and groups. | `whoami` `id` `sudo` `su` `useradd` `usermod` `passwd` `groupadd` |
| 🔐 | **[Permissions & Attributes](notes/permissions-attributes.md)** | Control who can read, write and run files, plus special attributes and capabilities. | `chmod` `chown` `chgrp` `lsattr` `chattr` `getcap` `setcap` |
| 🐚 | **[Shell & Environment](notes/shell-environment.md)** | Shell settings, environment variables, aliases and handy history shortcuts. | `bash` `export` `alias` `!$` `!?` `Ctrl + L` |
| ⏱️ | **[Processes & Scheduling](notes/processes-scheduling.md)** | See what's running, limit or repeat commands, and schedule jobs with cron. | `ps` `sleep` `timeout` `watch` `crontab` |
| 🌐 | **[Networking](notes/networking.md)** | Network interfaces, open ports and sockets, and raw connections with netcat. | `hostname` `ifconfig` `iwconfig` `ss` `lsof` `nc` `ncat` |
| 🔑 | **[SSH & Remote Access](notes/ssh-remote-access.md)** | Connect to remote machines and manage SSH keys. | `ssh` `sshpass` `ssh-keygen` `ssh-copy-id` |
| 🧬 | **[Binary, Encoding & Compression](notes/binary-encoding-compression.md)** | Inspect binary data, convert between formats, hash files and work with archives. | `strings` `xxd` `ghex` `base64` `md5sum` `bc` `7z` |
| 📦 | **[System & Packages](notes/system-packages.md)** | Update the system, manage packages and check system info. | `apt` `parrot-upgrade` `reboot` `neofetch` |
| 🌿 | **[Git](notes/git.md)** | Version control: clone projects, explore history, work with branches and publish changes. | `git clone` `git log` `git show` `git branch` `git checkout` `git tag` `git add` `git commit` `git push` |

### 🐚 Bash Scripting

| | Category | What's inside | Commands |
|:-:|:--|:--|:--|
| 📜 | **[Script Basics](notes/script-basics.md)** | The building blocks of every script: the shebang, exit codes, command substitution and subshells. | `#!/bin/bash` `exit` `$()` `(command)` `#` |
| 📦 | **[Variables & Arithmetic](notes/variables-arithmetic.md)** | Store values in variables, read them back and do math with them. | `variable="Hello"` `$variable or ${variable}` `${color_variable}` `declare` `let` `$(( ))` `read` `$RANDOM` `%` |
| 🎯 | **[Arguments & Options](notes/arguments-options.md)** | Read what's passed to your script: positional arguments and flags parsed with getopts. | `$0` `$1, $2...` `$#` `$*` `getopts` |
| 🔀 | **[Conditionals](notes/conditionals.md)** | Make decisions with if and case. | `if` `case` |
| 🔁 | **[Loops & Sequences](notes/loops-sequences.md)** | Repeat work with for and while, and generate sequences to loop over. | `for` `while` `seq` `{0000..9999}` `break` |
| 🧩 | **[Functions & Signals](notes/functions-signals.md)** | Group commands into functions and react to signals like Ctrl+C. | `function name(){ commands }` `trap` |
| ⚙️ | **[Jobs, Temp Files & Terminal](notes/jobs-temp-files-terminal.md)** | Wait for background jobs, set time limits, create temp files and control the cursor. | `wait` `mktemp` `tput` |
| 🌐 | **[Networking in Bash](notes/networking-in-bash.md)** | Open TCP connections from pure Bash and make HTTP requests. | `/dev/tcp/$ip/$port` `curl` |
| 🛠️ | **[Helper Tools](notes/helper-tools.md)** | Handy tools for reading and prettifying code while you script. | `batcat` `js-beautify` |

## 🔤 A–Z index

| Command | What it does | Category |
|:--|:--|:--|
| [`2>&1`](notes/pipes-redirection-operators.md#cmd-2-1) | Redirects stderr to stdout, showing everything together | 🔀 Pipes, Redirection & Operators |
| [`2>/dev/null`](notes/pipes-redirection-operators.md#cmd-2-dev-null) | Sends errors (stderr) to /dev/null so they aren't shown | 🔀 Pipes, Redirection & Operators |
| [`7z`](notes/binary-encoding-compression.md#cmd-7z) | Compresses and extracts .7z archives | 🧬 Binary, Encoding & Compression |
| [`alias`](notes/shell-environment.md#cmd-alias) | Creates a shortcut so a short word runs a longer command | 🐚 Shell & Environment |
| [`apt`](notes/system-packages.md#cmd-apt) | Debian's package manager: refreshes the package list (update) and installs available updates (upgrade) | 📦 System & Packages |
| [`awk`](notes/text-processing.md#cmd-awk) | Processes and filters text by columns | ✂️ Text Processing |
| [`base64`](notes/binary-encoding-compression.md#cmd-base64) | Encodes text or a file to Base64, or decodes it back to its original form, depending on the flag | 🧬 Binary, Encoding & Compression |
| [`bash`](notes/shell-environment.md#cmd-bash) | Bash, the shell that runs what you type; launching it starts a new shell, useful to get an interactive shell, run scripts or escape restricted shells | 🐚 Shell & Environment |
| [`batcat`](notes/helper-tools.md#cmd-batcat) | Shows a file like cat, but with syntax highlighting and line numbers | 🛠️ Helper Tools |
| [`bc`](notes/binary-encoding-compression.md#cmd-bc) | Terminal calculator; does arithmetic and converts numbers between bases (hexadecimal, decimal) | 🧬 Binary, Encoding & Compression |
| [`break`](notes/loops-sequences.md#cmd-break) | Leaves only the current loop; the script keeps running after it | 🔁 Loops & Sequences |
| [`case`](notes/conditionals.md#cmd-case) | Compares a variable against several patterns and runs the block that matches; closed with esac | 🔀 Conditionals |
| [`cat`](notes/viewing-editing-files.md#cmd-cat) | Prints a file's contents to the terminal | 📝 Viewing & Editing Files |
| [`cd`](notes/navigation-files.md#cmd-cd) | Changes directory | 📁 Navigation & Files |
| [`chattr`](notes/permissions-attributes.md#cmd-chattr) | Changes a file's special attributes (for example making it immutable) | 🔐 Permissions & Attributes |
| [`chgrp`](notes/permissions-attributes.md#cmd-chgrp) | Changes the group that owns a file or folder | 🔐 Permissions & Attributes |
| [`chmod`](notes/permissions-attributes.md#cmd-chmod) | Changes the permissions of a file or folder; + adds and - removes a permission | 🔐 Permissions & Attributes |
| [`chown`](notes/permissions-attributes.md#cmd-chown) | Changes the owner and/or owning group of a file or folder | 🔐 Permissions & Attributes |
| [`column`](notes/text-processing.md#cmd-column) | Arranges incoming text into aligned columns, like a table | ✂️ Text Processing |
| [`command`](notes/searching.md#cmd-command) | With -v, shows the path of a command, similar to which | 🔍 Searching |
| [`cp`](notes/navigation-files.md#cmd-cp) | Copies files or folders from one place to another | 📁 Navigation & Files |
| [`crontab`](notes/processes-scheduling.md#cmd-crontab) | Lets you view, create and edit a user's Cron jobs (scheduled tasks) | ⏱️ Processes & Scheduling |
| [`Ctrl + L`](notes/shell-environment.md#cmd-ctrl-l) | Shortcut that clears the terminal screen without losing your history | 🐚 Shell & Environment |
| [`curl`](notes/networking-in-bash.md#cmd-curl) | Sends requests to a URL from the terminal (HTTP, HTTPS, etc.) and shows the response | 🌐 Networking in Bash |
| [`cut`](notes/text-processing.md#cmd-cut) | Extracts parts of a line of text, splitting it by a delimiter | ✂️ Text Processing |
| [`declare`](notes/variables-arithmetic.md#cmd-declare) | Declares variables with attributes, for example making them integers | 📦 Variables & Arithmetic |
| [`diff`](notes/viewing-editing-files.md#cmd-diff) | Compares two files line by line and shows the differences between them | 📝 Viewing & Editing Files |
| [`disown`](notes/pipes-redirection-operators.md#cmd-disown) | Detaches a background process from the terminal so it keeps running after you close it | 🔀 Pipes, Redirection & Operators |
| [`echo`](notes/text-processing.md#cmd-echo) | Prints text or a variable's value to the terminal | ✂️ Text Processing |
| [`exec`](notes/pipes-redirection-operators.md#cmd-exec) | Manipulates the current session's file descriptors (open, close, redirect) | 🔀 Pipes, Redirection & Operators |
| [`exit`](notes/script-basics.md#cmd-exit) | Closes the current session or leaves an elevated one (like root); in a script, ends it with an exit code: 0 if it worked, anything else if it failed | 📜 Script Basics |
| [`export`](notes/shell-environment.md#cmd-export) | Turns a variable into an environment variable, available to other processes started from that terminal | 🐚 Shell & Environment |
| [`file`](notes/navigation-files.md#cmd-file) | Analyzes a file and tells you what kind of content it has, regardless of its extension | 📁 Navigation & Files |
| [`find`](notes/searching.md#cmd-find) | Searches for files and folders by criteria (name, type, permissions, date, etc.) | 🔍 Searching |
| [`for`](notes/loops-sequences.md#cmd-for) | Loops over a list of items one by one, running a block of code for each | 🔁 Loops & Sequences |
| [`function name(){ commands }`](notes/functions-signals.md#cmd-function-name-commands) | Defines a custom function that groups several commands under one name | 🧩 Functions & Signals |
| [`getcap`](notes/permissions-attributes.md#cmd-getcap) | Shows the capabilities assigned to a file | 🔐 Permissions & Attributes |
| [`getopts`](notes/arguments-options.md#cmd-getopts) | Processes the options a script receives (-m, -h...) one at a time; usually used inside a while loop | 🎯 Arguments & Options |
| [`ghex`](notes/binary-encoding-compression.md#cmd-ghex) | Hex editor with a graphical interface to view and modify a file's bytes | 🧬 Binary, Encoding & Compression |
| [`git add`](notes/git.md#cmd-git-add) | Adds files to the staging area so they're included in the next commit | 🌿 Git |
| [`git branch`](notes/git.md#cmd-git-branch) | Creates, lists, deletes and renames branches; it doesn't switch or merge them | 🌿 Git |
| [`git checkout`](notes/git.md#cmd-git-checkout) | Switches to another branch or takes the project back to a previous commit | 🌿 Git |
| [`git clone`](notes/git.md#cmd-git-clone) | Downloads a full copy of a remote repository (like GitHub), with all its files and history | 🌿 Git |
| [`git commit`](notes/git.md#cmd-git-commit) | Saves the staged changes, creating a new version of the project in the local repo | 🌿 Git |
| [`git log`](notes/git.md#cmd-git-log) | Lists every commit in the project with its ID, author, date and message | 🌿 Git |
| [`git push`](notes/git.md#cmd-git-push) | Uploads commits from the local repo to the remote repo | 🌿 Git |
| [`git show`](notes/git.md#cmd-git-show) | Shows the details and changes applied in a specific commit | 🌿 Git |
| [`git tag`](notes/git.md#cmd-git-tag) | Lists all the tags in the repo; a tag is a name that permanently marks a specific commit | 🌿 Git |
| [`grep`](notes/searching.md#cmd-grep) | Searches and filters lines of text that match a pattern | 🔍 Searching |
| [`groupadd`](notes/users-groups.md#cmd-groupadd) | Creates a new group on the system | 👤 Users & Groups |
| [`head`](notes/viewing-editing-files.md#cmd-head) | Shows the first lines of a file or text (10 by default) | 📝 Viewing & Editing Files |
| [`hostname`](notes/networking.md#cmd-hostname) | Shows or changes the machine's network name | 🌐 Networking |
| [`id`](notes/users-groups.md#cmd-id) | Shows user info: UID, GID and the groups they belong to | 👤 Users & Groups |
| [`if`](notes/conditionals.md#cmd-if) | Runs a block if the condition is true and another one (else) if it isn't; closed with fi | 🔀 Conditionals |
| [`ifconfig`](notes/networking.md#cmd-ifconfig) | Shows and configures network interfaces (the IP of each card) | 🌐 Networking |
| [`iwconfig`](notes/networking.md#cmd-iwconfig) | Like ifconfig, but for wireless (Wi-Fi) interfaces | 🌐 Networking |
| [`js-beautify`](notes/helper-tools.md#cmd-js-beautify) | Formats minified JavaScript or JSON so it's readable (line breaks and indentation) | 🛠️ Helper Tools |
| [`let`](notes/variables-arithmetic.md#cmd-let) | Does arithmetic on variables | 📦 Variables & Arithmetic |
| [`ls`](notes/navigation-files.md#cmd-ls) | Lists the files and folders in the current directory | 📁 Navigation & Files |
| [`lsattr`](notes/permissions-attributes.md#cmd-lsattr) | Shows a file's special attributes (beyond the normal permissions) | 🔐 Permissions & Attributes |
| [`lsof`](notes/networking.md#cmd-lsof) | Lists the files opened by running processes, including network connections | 🌐 Networking |
| [`md5sum`](notes/binary-encoding-compression.md#cmd-md5sum) | Calculates the MD5 hash of a file or input, useful to check whether its content has changed | 🧬 Binary, Encoding & Compression |
| [`mkdir`](notes/navigation-files.md#cmd-mkdir) | Creates a new folder | 📁 Navigation & Files |
| [`mktemp`](notes/jobs-temp-files-terminal.md#cmd-mktemp) | Creates a temporary file with a unique name, avoiding clashes with other files | ⚙️ Jobs, Temp Files & Terminal |
| [`more`](notes/viewing-editing-files.md#cmd-more) | Shows a command's output or a file one page at a time (space to advance, q to quit) | 📝 Viewing & Editing Files |
| [`nano`](notes/viewing-editing-files.md#cmd-nano) | Simple text editor in the terminal | 📝 Viewing & Editing Files |
| [`nc`](notes/networking.md#cmd-nc) | Netcat: creates manual TCP/UDP connections to send and receive data, scan ports or open remote shells | 🌐 Networking |
| [`ncat`](notes/networking.md#cmd-ncat) | Improved netcat (from the Nmap project) with SSL/TLS encryption and authentication support | 🌐 Networking |
| [`neofetch`](notes/system-packages.md#cmd-neofetch) | Shows system info (kernel, RAM, CPU, distro logo) in a visual way | 📦 System & Packages |
| [`parrot-upgrade`](notes/system-packages.md#cmd-parrot-upgrade) | Safely upgrades Parrot OS without breaking its own components | 📦 System & Packages |
| [`passwd`](notes/users-groups.md#cmd-passwd) | Sets or changes a user's password | 👤 Users & Groups |
| [`ps`](notes/processes-scheduling.md#cmd-ps) | Shows the processes running on the system | ⏱️ Processes & Scheduling |
| [`pwd`](notes/navigation-files.md#cmd-pwd) | Shows the full path of the current directory | 📁 Navigation & Files |
| [`read`](notes/variables-arithmetic.md#cmd-read) | Saves what the user types into a variable | 📦 Variables & Arithmetic |
| [`reboot`](notes/system-packages.md#cmd-reboot) | Restarts the machine | 📦 System & Packages |
| [`rev`](notes/viewing-editing-files.md#cmd-rev) | Reverses the characters of each line, showing the text backwards | 📝 Viewing & Editing Files |
| [`rm`](notes/navigation-files.md#cmd-rm) | Deletes files or folders | 📁 Navigation & Files |
| [`sed`](notes/text-processing.md#cmd-sed) | Finds, replaces, deletes or modifies text in a file or stream, usually with regular expressions | ✂️ Text Processing |
| [`seq`](notes/loops-sequences.md#cmd-seq) | Generates a sequence of numbers within a range, handy for loops | 🔁 Loops & Sequences |
| [`setcap`](notes/permissions-attributes.md#cmd-setcap) | Assigns specific capabilities to a file without granting full root privileges | 🔐 Permissions & Attributes |
| [`sleep`](notes/processes-scheduling.md#cmd-sleep) | Pauses for a given number of seconds | ⏱️ Processes & Scheduling |
| [`sort`](notes/text-processing.md#cmd-sort) | Sorts the lines of a file or text, alphabetically or numerically | ✂️ Text Processing |
| [`sponge`](notes/text-processing.md#cmd-sponge) | Reads all of its input before writing it to a file, avoiding problems when overwriting the same file you're reading | ✂️ Text Processing |
| [`ss`](notes/networking.md#cmd-ss) | Shows information about active network sockets, a modern alternative to netstat | 🌐 Networking |
| [`ssh`](notes/ssh-remote-access.md#cmd-ssh) | Connects remotely and securely to another machine over the network, using a password or an SSH key | 🔑 SSH & Remote Access |
| [`ssh-copy-id`](notes/ssh-remote-access.md#cmd-ssh-copy-id) | Copies your SSH public key to a remote server's authorized_keys | 🔑 SSH & Remote Access |
| [`ssh-keygen`](notes/ssh-remote-access.md#cmd-ssh-keygen) | Generates an SSH key pair (public and private) to log in without a password | 🔑 SSH & Remote Access |
| [`sshpass`](notes/ssh-remote-access.md#cmd-sshpass) | Passes the SSH password directly in the command; handy for automation | 🔑 SSH & Remote Access |
| [`stat`](notes/navigation-files.md#cmd-stat) | Shows detailed info about a file or directory: permissions, size and access/modification dates | 📁 Navigation & Files |
| [`strings`](notes/binary-encoding-compression.md#cmd-strings) | Shows the readable text strings (ASCII) inside a binary file; useful for finding hidden info | 🧬 Binary, Encoding & Compression |
| [`su`](notes/users-groups.md#cmd-su) | Switches to another user in the terminal, asking for their password | 👤 Users & Groups |
| [`sudo`](notes/users-groups.md#cmd-sudo) | Runs a single command with administrator privileges without switching users | 👤 Users & Groups |
| [`tail`](notes/viewing-editing-files.md#cmd-tail) | Shows the last lines of a file (10 by default), useful for logs | 📝 Viewing & Editing Files |
| [`tee`](notes/text-processing.md#cmd-tee) | Shows a command's output on screen and saves it to a file at the same time | ✂️ Text Processing |
| [`timeout`](notes/processes-scheduling.md#cmd-timeout) | Runs a command and kills it automatically if it goes over the given time | ⏱️ Processes & Scheduling |
| [`touch`](notes/navigation-files.md#cmd-touch) | Creates an empty file, or updates its modification date if it already exists | 📁 Navigation & Files |
| [`tput`](notes/jobs-temp-files-terminal.md#cmd-tput) | Controls the terminal, for example hiding or showing the cursor | ⚙️ Jobs, Temp Files & Terminal |
| [`tr`](notes/text-processing.md#cmd-tr) | Translates or replaces characters of the incoming text with others | ✂️ Text Processing |
| [`trap`](notes/functions-signals.md#cmd-trap) | Catches a signal (like Ctrl+C) and runs a function instead of stopping the script right away | 🧩 Functions & Signals |
| [`uniq`](notes/text-processing.md#cmd-uniq) | Removes consecutive duplicate lines; usually used after sort | ✂️ Text Processing |
| [`useradd`](notes/users-groups.md#cmd-useradd) | Creates a new user on the system | 👤 Users & Groups |
| [`usermod`](notes/users-groups.md#cmd-usermod) | Modifies an existing user's properties (group, home, shell) | 👤 Users & Groups |
| [`variable="Hello"`](notes/variables-arithmetic.md#cmd-variable-hello) | Declares a variable and assigns it some text (no spaces around the =) | 📦 Variables & Arithmetic |
| [`vi`](notes/viewing-editing-files.md#cmd-vi) | Advanced, powerful text editor with a steeper learning curve than nano | 📝 Viewing & Editing Files |
| [`wait`](notes/jobs-temp-files-terminal.md#cmd-wait) | Waits for one or more background processes to finish before continuing | ⚙️ Jobs, Temp Files & Terminal |
| [`watch`](notes/processes-scheduling.md#cmd-watch) | Runs a command repeatedly at regular intervals and shows its updated output | ⏱️ Processes & Scheduling |
| [`which`](notes/searching.md#cmd-which) | Shows where a command or program is installed | 🔍 Searching |
| [`while`](notes/loops-sequences.md#cmd-while) | Repeats a block of code while a condition is true | 🔁 Loops & Sequences |
| [`whoami`](notes/users-groups.md#cmd-whoami) | Shows the name of the user you're currently logged in as | 👤 Users & Groups |
| [`xargs`](notes/searching.md#cmd-xargs) | Takes a command's output and uses it as the arguments of another command | 🔍 Searching |
| [`xxd`](notes/binary-encoding-compression.md#cmd-xxd) | Shows a file's contents in hexadecimal | 🧬 Binary, Encoding & Compression |
| [`!$`](notes/shell-environment.md#cmd-sym-33-36) | Stands for the last argument of the previous command, so you can reuse it | 🐚 Shell & Environment |
| [`!?`](notes/shell-environment.md#cmd-sym-33-63) | Finds the most recent command in your history containing the given text and runs it again | 🐚 Shell & Environment |
| [`#`](notes/script-basics.md#cmd-sym-35) | Comments out a line so it doesn't run; handy to hide debug traces without deleting them | 📜 Script Basics |
| [`#!/bin/bash`](notes/script-basics.md#cmd-bin-bash) | Shebang: the first line of a script, telling the system to run it with Bash | 📜 Script Basics |
| [`$#`](notes/arguments-options.md#cmd-sym-36-35) | Holds the number of arguments passed on the command line | 🎯 Arguments & Options |
| [`$(( ))`](notes/variables-arithmetic.md#cmd-sym-36-40-40-41-41) | Arithmetic expansion: does the math inside and returns the result | 📦 Variables & Arithmetic |
| [`$()`](notes/script-basics.md#cmd-sym-36-40-41) | Runs the command inside the parentheses and uses its output (command substitution) | 📜 Script Basics |
| [`$*`](notes/arguments-options.md#cmd-sym-36-42) | Holds all the arguments passed on the command line in a single variable | 🎯 Arguments & Options |
| [`$0`](notes/arguments-options.md#cmd-0) | Holds the name of the script as it was called from the terminal | 🎯 Arguments & Options |
| [`$1, $2...`](notes/arguments-options.md#cmd-1-2) | The first, second (and so on) argument passed on the command line | 🎯 Arguments & Options |
| [`$RANDOM`](notes/variables-arithmetic.md#cmd-random) | Returns a random number between 0 and 32767 each time it's read | 📦 Variables & Arithmetic |
| [`$variable or ${variable}`](notes/variables-arithmetic.md#cmd-variable-or-variable) | Reads a variable's value; the braces mark where the name ends when it's stuck to other text | 📦 Variables & Arithmetic |
| [`${color_variable}`](notes/variables-arithmetic.md#cmd-color-variable) | Variables that hold ANSI color codes; put one before the text to color it and close with the end-color variable | 📦 Variables & Arithmetic |
| [`%`](notes/variables-arithmetic.md#cmd-sym-37) | Modulo: returns the remainder of a division; handy to limit a range or tell even (0) from odd (1) | 📦 Variables & Arithmetic |
| [`&`](notes/pipes-redirection-operators.md#cmd-sym-38) | Runs the command in the background, leaving the terminal free | 🔀 Pipes, Redirection & Operators |
| [`&&`](notes/pipes-redirection-operators.md#cmd-sym-38-38) | Runs the next command only if the previous one succeeded | 🔀 Pipes, Redirection & Operators |
| [`&>/dev/null`](notes/pipes-redirection-operators.md#cmd-dev-null) | Sends both normal output and errors to /dev/null, hiding everything | 🔀 Pipes, Redirection & Operators |
| [`(command)`](notes/script-basics.md#cmd-command) | Runs the command in a subshell, a child process separate from the main script | 📜 Script Basics |
| [`*`](notes/navigation-files.md#cmd-sym-42) | Wildcard that matches anything, to select several files at once | 📁 Navigation & Files |
| [`/dev/tcp/$ip/$port`](notes/networking-in-bash.md#cmd-dev-tcp-ip-port) | Special Bash path that opens a TCP connection to an IP and port as if it were a file, no netcat needed | 🌐 Networking in Bash |
| [`;`](notes/pipes-redirection-operators.md#cmd-sym-59) | Runs commands in sequence whether or not the previous one failed | 🔀 Pipes, Redirection & Operators |
| [`>`](notes/pipes-redirection-operators.md#cmd-sym-62) | Redirects output to a file, overwriting its contents | 🔀 Pipes, Redirection & Operators |
| [`>>`](notes/pipes-redirection-operators.md#cmd-sym-62-62) | Redirects output to a file, appending it to the end | 🔀 Pipes, Redirection & Operators |
| [`{0000..9999}`](notes/loops-sequences.md#cmd-0000-9999) | Brace expansion: generates a sequence of values (here 0000 to 9999), useful as a counter in loops | 🔁 Loops & Sequences |
| [`\|`](notes/pipes-redirection-operators.md#cmd-sym-124) | Pipe: sends one command's output as the next command's input | 🔀 Pipes, Redirection & Operators |
| [`\|\|`](notes/pipes-redirection-operators.md#cmd-sym-124-124) | Runs the next command only if the previous one failed | 🔀 Pipes, Redirection & Operators |

## 🛠️ How to update

The data lives in [`data/`](data): [`categories.csv`](data/categories.csv), [`commands.csv`](data/commands.csv) and [`parameters.csv`](data/parameters.csv). After editing them, run:

```bash
python3 scripts/build.py
```

This rebuilds this README, the notes in [`notes/`](notes) and the web page in [`docs/`](docs).

> 💡 To publish the web page: **Settings → Pages → Branch `main` / folder `/docs`**.
