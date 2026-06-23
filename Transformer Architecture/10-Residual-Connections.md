# Residual Connections

Purpose:

Preserve original information.

---

Formula

```text
R = X + F(X)
```

---

Attention Residual

```text
R1

=
X + AttentionOutput
```

Shape:

```text
3 × 4096
```

---

Why?

Without residuals:

```text
Deep networks become unstable.
```

Residuals create:

```text
Shortcut Paths
```

```text
X
│
├────────────┐
│            │
▼            │
Attention    │
│            │
▼            │
Add ◄────────┘
```

Next:

[[11-LayerNorm]]