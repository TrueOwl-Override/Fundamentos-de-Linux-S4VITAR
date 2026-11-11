# 🔀 Conditionals

> Make decisions with if and case.

**Bash Scripting** · **2** commands · **11** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Command | What it does |
|:--|:--|
| [`if`](#cmd-if) | Runs a block if the condition is true and another one (else) if it isn't; closed with fi |
| [`case`](#cmd-case) | Compares a variable against several patterns and runs the block that matches; closed with esac |

---

<a id="cmd-if"></a>

## `if`

Runs a block if the condition is true and another one (else) if it isn't; closed with fi

```bash
if [ $n -eq 1 ]; then echo "one"; else echo "other"; fi
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `-eq` | Checks whether two numbers are equal | `if [ $a -eq $b ]; then echo "equal"; fi` |
| `-ne` | Checks whether two numbers are different (not equal) | `if [ $a -ne $b ]; then echo "different"; fi` |
| `-gt` | Checks whether the first number is greater than the second | `if [ $a -gt $b ]; then echo "greater"; fi` |
| `-lt` | Checks whether the first number is less than the second | `if [ $a -lt $b ]; then echo "less"; fi` |
| `-le` | Checks whether the first number is less than or equal to the second | `if [ $a -le $b ]; then echo "less or equal"; fi` |
| `==` | Compares two text strings to check they're equal | `if [ "$choice" == "even" ]; then echo "even"; fi` |
| `!` | Negates the condition: [ ! $a -le 0 ] is the same as [ $a -gt 0 ] | `if [ ! "$money" -le 0 ]; then echo "still have money"; fi` |
| `-f` | Checks whether the file exists and is a regular file (not a folder) | `if [ -f file.txt ]; then echo "exists"; fi` |
| `elif` | Inside an if, checks another condition when the previous one wasn't met (else if) | `if [ $n -eq 1 ]; then echo "one"; elif [ $n -eq 2 ]; then echo "two"; else echo "other"; fi` |
| `else` | Runs a block when none of the if or elif conditions were met; goes right before fi | `if [ -f file.txt ]; then echo "exists"; else echo "missing"; fi` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-case"></a>

## `case`

Compares a variable against several patterns and runs the block that matches; closed with esac

```bash
case $arg in m) echo "option m";; esac
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `m) command;;` | Defines a pattern inside case and the block to run if it matches; ;; closes that block | `case $arg in m) echo "option m";; esac` |

<sub>[⬆ Back to top](#commands)</sub>
