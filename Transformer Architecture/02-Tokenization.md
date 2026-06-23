# Tokenization

## Goal

Convert text into token IDs.

Input:

```text
I love cats
```

Output:

```python
[15, 92, 344]
```

Shape:

```text
(N)

3
```

---

## Why Token IDs?

Neural networks operate on numbers.

Not strings.

Instead of:

```text
"I"
```

we use:

```text
15
```

---

## Visualization

```text
"I"      -> 15
"love"   -> 92
"cats"   -> 344
```

---

## Output Shape

```text
N
```

Where:

```text
N = number of tokens
```

Example:

```text
[15,92,344]

N=3
```

Next:

[[03-Embeddings]]