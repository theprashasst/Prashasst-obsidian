# Final Hidden State

After last transformer layer:

```text
H_final
```

Shape:

```text
N × D

3 × 4096
```

Example:

```text
h1
h2
h3
```

Each row belongs to one token.

---

For next token prediction:

Use only

```text
h3
```

Shape:

```text
1 × 4096
```

Next:

[[15-Logits]]