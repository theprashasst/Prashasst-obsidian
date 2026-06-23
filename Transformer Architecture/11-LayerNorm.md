# Layer Normalization

Purpose:

Keep activations stable.

---

Formula

For each token:

```text
x_norm

=
(x - mean)

/
sqrt(var + ε)
```

---

Shape

Input:

```text
N × D
```

Output:

```text
N × D
```

No shape change.

---

Example

```text
3 × 4096

↓

3 × 4096
```

Next:

[[12-FeedForward-Network]]