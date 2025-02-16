---
title: Úryvky programov
slug: uryvky-programov
publish: true
---

### 1. úloha
Podľa kódu programu vytvor platný vstupný súbor. Popíš ako bude vyzerať výstupný súbor alebo súbory.

```python
vstup = open('vstup.txt', 'r')
a = open('a.txt', 'w')
b = open('b.txt', 'w')

for m in vstup:
    m = m.strip()
    op, x, y = m.split(' ')
    x = int(x)
    y = int(y)

    if op == '!':
        r = x + y
        print('{} {}'.format(m, r), file=a)

    elif op == '?'
        r = x * y
        print('{} {}'.format(m, r), file=b)

vstup.close()
a.close()
b.close()
```

### 2. úloha
Usporiadaj riadky kódu programu do správneho poradia? Akú činnosť vykonáva opravený program?

Chýbajú v programe nejaké riadok kódu? Ak áno, doplň!

**1**
```python
if cifry[2] == '5' or cifry[2] == '6':
    n += 1
```

**2**
```python
for ziak in ziaci:
    meno, cifry = ziak.split(' ')
    mesiac = int(cifry[2:4])
```

**3**
```python
nar = []
if t < 1 or t > 12:
    return nar
```

**4**
```python
with open('skupina.txt', 'r') as subor:
    for meno in subor:
        ziaci.append(meno.rstrip())
```

**5**
```python
for ziak in ziaci:
    meno, cifry = ziak.split(' ')
```

**6**
```python
if mesiac > 50:
    mesiac -= 50
if mesiac == t:
    nar.append(meno)
```
