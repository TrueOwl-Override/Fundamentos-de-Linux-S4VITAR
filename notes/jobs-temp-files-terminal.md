# ⚙️ Jobs, Temp Files & Terminal

> Wait for background jobs, set time limits, create temp files and control the cursor.

**Bash Scripting** · **3** commands · **3** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Command | What it does |
|:--|:--|
| [`wait`](#cmd-wait) | Waits for one or more background processes to finish before continuing |
| [`mktemp`](#cmd-mktemp) | Creates a temporary file with a unique name, avoiding clashes with other files |
| [`tput`](#cmd-tput) | Controls the terminal, for example hiding or showing the cursor |

---

<a id="cmd-wait"></a>

## `wait`

Waits for one or more background processes to finish before continuing

```bash
sleep 5 & wait
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-mktemp"></a>

## `mktemp`

Creates a temporary file with a unique name, avoiding clashes with other files

```bash
mktemp
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `-d` | Creates a temporary folder instead of a file, with a unique name | `mktemp -d` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-tput"></a>

## `tput`

Controls the terminal, for example hiding or showing the cursor

```bash
tput civis
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `civis` | Hides the terminal cursor | `tput civis` |
| `cnorm` | Shows the terminal cursor again | `tput cnorm` |

<sub>[⬆ Back to top](#commands)</sub>
