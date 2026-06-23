# Token Sampling

Input

```text
Probabilities
```

Shape

```text
1 × Vocab
```

---

Methods

## Greedy

```text
argmax(p)
```

Choose largest probability.

---

## Sampling

Randomly sample using probabilities.

Produces:

```text
Next Token ID
```

---

Loop

Append token.

```text
N = N + 1
```

Run transformer again.

Continue until:

```text
EOS token
```

or

```text
Maximum Length
```