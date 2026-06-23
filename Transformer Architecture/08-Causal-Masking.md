# Causal Masking

Decoder models cannot see the future.

---

Example:

```text
I love cats
```

While predicting:

```text
love
```

Model cannot see:

```text
cats
```

---

Mask:

```text
0   -∞  -∞

0    0  -∞

0    0   0
```

Shape:

```text
N × N
```

---

Operation

```text
MaskedScores

=
Scores + Mask
```

---

Result

Future positions become:

```text
Softmax(-∞)=0
```

Impossible to attend.

---

Next:

[[09-Multi-Head-Attention]]