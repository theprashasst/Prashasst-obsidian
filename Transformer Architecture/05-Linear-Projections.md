# Linear Projections

## Prerequisites

- [[03-Embeddings]]
    
- [[04-Matrix-Multiplication]]
    

---

# Why Linear Projections Exist

Neural networks cannot directly understand the meaning of a vector.

Instead, they repeatedly transform vectors into new vector spaces.

These transformations are called:

```text
Linear Projections
```

A linear projection is simply:

```text
Output = Input × WeightMatrix
```

or

```text
Y = XW
```

---

# General Formula

Input:

```text
X

Shape:
N × Din
```

Weight:

```text
W

Shape:
Din × Dout
```

Output:

```text
Y = XW
```

Shape:

```text
(N × Din)

×

(Din × Dout)

=

N × Dout
```

---

# Visualization

Input Matrix

```text
X

N × Din
```

```text
          Din Features

      ┌───────────────┐
Token1│               │
Token2│               │
Token3│               │
      └───────────────┘
```

Weight Matrix

```text
W

Din × Dout
```

```text
          Output Features

       ┌──────────────┐
Feat1  │              │
Feat2  │              │
Feat3  │              │
       └──────────────┘
```

After multiplication:

```text
Y = XW
```

```text
N × Dout
```

---

# What Does The Weight Matrix Learn?

The weight matrix learns:

```text
How to combine input features
```

Suppose:

```text
X

=
[ height
  weight
  age ]
```

A learned projection might create:

```text
athletic_score
health_score
risk_score
```

from those inputs.

The model learns these combinations automatically.

---

# Example Using Transformer Embeddings

Embedding Output:

```text
X

Shape:

3 × 4
```

Example:

```text
        D=4

I      [1 2 3 4]

love   [5 6 7 8]

cats   [9 1 2 3]
```

---

Weight Matrix

```text
W

Shape:

4 × 4
```

```text
[ a b c d ]
[ e f g h ]
[ i j k l ]
[ m n o p ]
```

---

Projection

```text
Y = XW
```

Shape:

```text
(3 × 4)

×

(4 × 4)

=

3 × 4
```

Result:

```text
Y

3 × 4
```

The values change.

The shape remains the same.

---

# Geometric Interpretation

A projection can:

## Rotate

```text
↻
```

the vector space.

---

## Stretch

```text
←────→
```

certain directions.

---

## Compress

```text
→←
```

certain directions.

---

## Mix Features

Input feature:

```text
Feature 1
```

may influence

```text
Output Feature 3
```

through learned weights.

---

# Why Transformers Use So Many Projections

Transformers constantly ask:

```text
What information do I need?
```

```text
What information do I contain?
```

```text
What information should I send?
```

These become:

```text
Query Projection
Key Projection
Value Projection
```

Each is just another linear projection.

---

# Projection Examples Inside Attention

## Query Projection

```text
Q = XWq
```

Weight:

```text
Wq

D × Dh
```

---

## Key Projection

```text
K = XWk
```

Weight:

```text
Wk

D × Dh
```

---

## Value Projection

```text
V = XWv
```

Weight:

```text
Wv

D × Dh
```

---

# Shape Example

Suppose:

```text
N = 3
D = 4
Dh = 4
```

Input:

```text
X

3 × 4
```

Projection:

```text
Q = XWq
```

```text
(3×4)

×

(4×4)

=

3×4
```

Likewise:

```text
K = 3×4
V = 3×4
```

---

# Important Insight

The embeddings are the same for every token.

The projections create specialized versions of those embeddings.

```text
Embedding
     ↓
     X

     ├──Wq→ Q
     │
     ├──Wk→ K
     │
     └──Wv→ V
```

Same input.

Different learned weight matrices.

Different outputs.

---

# Summary

A linear projection is:

```text
Y = XW
```

Purpose:

```text
Transform information
```

Effects:

```text
Rotate feature space
Stretch feature space
Compress feature space
Mix features
Create new representations
```

Transformers use linear projections everywhere:

```text
Embeddings
↓
Q Projection
↓
K Projection
↓
V Projection
↓
Output Projection
↓
Feed Forward Layers
↓
Vocabulary Projection
```

Next:

[[06-Queries-Keys-Values]]