# Softmax

Formula

```text
softmax(xi)

=
e^xi

/

Σ e^xj
```

---

Input

```text
1 × 50000
```

Output

```text
1 × 50000
```

---

Properties

All values:

```text
0 ≤ p ≤ 1
```

and

```text
Σp = 1
```

Meaning:

Probability distribution over vocabulary.

Next:

[[17-Token-Sampling]]