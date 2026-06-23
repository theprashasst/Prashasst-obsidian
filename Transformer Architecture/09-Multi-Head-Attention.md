# Multi Head Attention

One head is limited.

GPT uses many heads.

---

Example

```text
D = 4096
H = 32
Dh = 128
```

Relationship:

```text
D = H × Dh
```

---

Each Head

```text
N × Dh

3 × 128
```

---

Head Outputs

```text
Head1
Head2
...
Head32
```

---

Concatenation

```text
Concat(
Head1
Head2
...
Head32
)
```

Shape:

```text
3 × 4096
```

---

Output Projection

Weight:

```text
Wo

4096 × 4096
```

Operation:

```text
MWo
```

Output:

```text
3 × 4096
```

Next:

[[10-Residual-Connections]]