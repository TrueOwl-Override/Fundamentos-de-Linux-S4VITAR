# ➗ Operators

> Assign, do math, compare numbers and text, and negate conditions.

**Bash Scripting** · **11** commands · **0** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Command | What it does |
|:--|:--|
| [`=`](#cmd-sym-61) | Assigns a value to a variable, or copies another variable's value (no spaces around it) |
| [`+=`](#cmd-sym-43-61) | Adds to what the variable already holds: sums with numbers (with let), appends with text |
| [`+ - *`](#cmd-sym-43-45-42) | Add, subtract and multiply inside $(( )) or let |
| [`%`](#cmd-sym-37) | Modulo: returns the remainder of a division; handy to limit a range or tell even (0) from odd (1) |
| [`-eq`](#cmd-eq) | Checks whether two numbers are equal |
| [`-ne`](#cmd-ne) | Checks whether two numbers are different (not equal) |
| [`-gt`](#cmd-gt) | Checks whether the first number is greater than the second |
| [`-lt`](#cmd-lt) | Checks whether the first number is less than the second |
| [`-le`](#cmd-le) | Checks whether the first number is less than or equal to the second |
| [`==`](#cmd-sym-61-61) | Compares two text strings to check they're equal |
| [`!`](#cmd-sym-33) | Negates the condition: [ ! $a -le 0 ] is the same as [ $a -gt 0 ] |

---

<a id="cmd-sym-61"></a>

## `=`

Assigns a value to a variable, or copies another variable's value (no spaces around it)

```bash
backup_bet=$initial_bet
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-43-61"></a>

## `+=`

Adds to what the variable already holds: sums with numbers (with let), appends with text

```bash
let counter+=1; bad_plays+="$random_number "
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-43-45-42"></a>

## `+ - *`

Add, subtract and multiply inside $(( )) or let

```bash
echo $((5 + 3)) $((5 - 3)) $((5 * 3))
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-37"></a>

## `%`

Modulo: returns the remainder of a division; handy to limit a range or tell even (0) from odd (1)

```bash
echo $(($RANDOM % 37))
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-eq"></a>

## `-eq`

Checks whether two numbers are equal

```bash
if [ $a -eq $b ]; then echo "equal"; fi
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-ne"></a>

## `-ne`

Checks whether two numbers are different (not equal)

```bash
if [ $a -ne $b ]; then echo "different"; fi
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-gt"></a>

## `-gt`

Checks whether the first number is greater than the second

```bash
if [ "$money" -gt "$max_money" ]; then echo "new max"; fi
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-lt"></a>

## `-lt`

Checks whether the first number is less than the second

```bash
if [ $a -lt $b ]; then echo "less"; fi
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-le"></a>

## `-le`

Checks whether the first number is less than or equal to the second

```bash
if [ $a -le $b ]; then echo "less or equal"; fi
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-61-61"></a>

## `==`

Compares two text strings to check they're equal

```bash
if [ "$choice" == "even" ]; then echo "even"; fi
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-33"></a>

## `!`

Negates the condition: [ ! $a -le 0 ] is the same as [ $a -gt 0 ]

```bash
if [ ! "$money" -le 0 ]; then echo "still have money"; fi
```

<sub>[⬆ Back to top](#commands)</sub>
