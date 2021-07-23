# fluent-notes

another note taking experiment

## algorithm test suite

### double line break on load

```
toto

titi
```

```
toto
---
titi
```

### double line break on enter

```
toto(enter)
titi
```

```
toto
---
(cursor)titi
```

### start with a line break on load

```

toto
```

```

---
toto
```

### start with a line break on enter

```
(enter)toto
```

```

---
(cursor)toto
```

### triple line break and more

```
toto


titi
```

```
toto
---
titi
```

### backspace at start

```
toto
---
(backspace)titi
```

```
toto
(cursor)titi
```

### backspace at start with previous empty

```
toto
---
---
(backspace)titi
```

```
toto
---
(cursor)titi
```

### delete at end

```
toto(delete)
---
titi
```

```
toto
(cursor)titi
```

### delete at end with following empty

```
toto(delete)
---
---
titi
```

```
toto(cursor)
----
titi
```

### delete the first line (not correctly handled)

```
(delete)t
titi
```

actual:

```

----
(cursor)titi
```

expected:

???
