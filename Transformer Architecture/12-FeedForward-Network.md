# Feed Forward Network

After attention.

Every token independently passes through a small neural network.

---

First Projection

```text
W1

4096 × 16384
```

Operation:

```text
H = XW1
```

Shape:

```text
3 × 16384
```

---

Activation

```text
GELU(H)
```

Shape unchanged.

---

Second Projection

```text
W2

16384 × 4096
```

Operation:

```text
FFN
=
GELU(H)W2
```

Shape:

```text
3 × 4096
```

---

Pipeline

```text
4096

↓

16384

↓

GELU

↓

4096
```

Next:

[[13-Transformer-Layer]]