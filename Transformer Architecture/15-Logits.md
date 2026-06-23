# Logits

Vocabulary Projection

Weight:

```text
W_vocab
```

Shape:

```text
4096 × 50000
```

Operation:

```text
logits

=
h3W_vocab
```

Shapes:

```text
(1×4096)

×

(4096×50000)

=

1×50000
```

---

Meaning

One score for every vocabulary token.

Next:

[[16-Softmax]]