# 📜 Script Basics

> The building blocks of every script: the shebang, exit codes, command substitution and subshells.

**Bash Scripting** · **4** commands · **2** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Command | What it does |
|:--|:--|
| [`#!/bin/bash`](#cmd-bin-bash) | Shebang: the first line of a script, telling the system to run it with Bash |
| [`exit`](#cmd-exit) | Closes the current session or leaves an elevated one (like root); in a script, ends it with an exit code: 0 if it worked, anything else if it failed |
| [`$()`](#cmd-sym-36-40-41) | Runs the command inside the parentheses and uses its output (command substitution) |
| [`(command)`](#cmd-command) | Runs the command in a subshell, a child process separate from the main script |

---

<a id="cmd-bin-bash"></a>

## `#!/bin/bash`

Shebang: the first line of a script, telling the system to run it with Bash

```bash
#!/bin/bash   (first line of script.sh)
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-exit"></a>

## `exit`

Closes the current session or leaves an elevated one (like root); in a script, ends it with an exit code: 0 if it worked, anything else if it failed

```bash
exit 0
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `0` | Ends the script with exit code 0, signalling success | `exit 0` |
| `1` | Ends the script with exit code 1, signalling an error | `exit 1` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-36-40-41"></a>

## `$()`

Runs the command inside the parentheses and uses its output (command substitution)

```bash
echo "I'm in $(pwd)"
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-command"></a>

## `(command)`

Runs the command in a subshell, a child process separate from the main script

```bash
(ping -c 1 192.168.1.1) &
```

<sub>[⬆ Back to top](#commands)</sub>
