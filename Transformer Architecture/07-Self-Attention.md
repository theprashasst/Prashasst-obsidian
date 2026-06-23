# Self Attention

Core Formula:

```text
Attention(Q,K,V)

=
Softmax(
QKᵀ / √Dh
)
V
```

---

# Step 1

Scores:

```text
Scores = QKᵀ
```

Shapes:

```text
Q   = 3 × 4
Kᵀ  = 4 × 3

Scores

= 3 × 3
```

---

## Visualization

```text
          Referenced Token

           I love cats

Query I    ● ● ●

Query love ● ● ●

Query cats ● ● ●
```

---

Meaning:

```text
Scores[i,j]

=
How much token i looks at token j
```

---

## Scaling

Actual Transformers use:

```text
Scores = QKᵀ / √Dh
```

Reason:

Prevent huge values.

---

Next:

[[08-Causal-Masking]]