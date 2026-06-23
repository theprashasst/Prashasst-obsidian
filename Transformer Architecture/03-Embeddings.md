# Embeddings

## Purpose

Convert token IDs into vectors.

---

## Embedding Matrix

Symbol:

```text
E
```

Shape:

```text
Vocab × D
```

Example:

```text
50000 × 4
```

---

## Visualization

```text
E

       D=4
     ┌────────────┐
id0  │            │
id1  │            │
id2  │            │
...  │            │
344  │0.1 0.3 0.8 0.2│
...  │            │
     └────────────┘
```

Each row stores a learned vector.

---

## Lookup

Operation:

```text
X = E[input_ids]
```

Input:

```python
[15,92,344]
```

Output:

```text
X
```

Shape:

```text
N × D

3 × 4
```

---

## Interpretation

Rows:

```text
Tokens
```

Columns:

```text
Features
```

```text
      D=4
     ┌───────────┐
I    │           │
love │           │
cats │           │
     └───────────┘
```

Next:

[[04-Matrix-Multiplication]]