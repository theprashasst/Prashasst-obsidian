# Queries Keys Values

Input:

```text
X

Shape:
N × D
```

Example:

```text
3 × 4
```

---

## Query Projection

Weight:

```text
Wq
```

Shape:

```text
D × Dh
```

Operation:

```text
Q = XWq
```

---

## Key Projection

Weight:

```text
Wk
```

Operation:

```text
K = XWk
```

---

## Value Projection

Weight:

```text
Wv
```

Operation:

```text
V = XWv
```

---

## Shape Flow

```text
X

3 × 4

↓

Wq

Q

3 × 4

↓

Wk

K

3 × 4

↓

Wv

V

3 × 4
```

---

## Meaning

Query

```text
What am I looking for?
```

Key

```text
What information do I contain?
```

Value

```text
What information should I send?
```

Next:

[[07-Self-Attention]]