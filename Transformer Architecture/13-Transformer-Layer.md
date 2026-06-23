# Transformer Layer

Complete Block

```text
Input

↓

Multi Head Attention

↓

Residual

↓

LayerNorm

↓

Feed Forward

↓

Residual

↓

LayerNorm

↓

Output
```

---

Shape

```text
N × D
```

never changes.

Example:

```text
3 × 4096

↓

3 × 4096
```

---

One layer changes meaning.

Not shape.