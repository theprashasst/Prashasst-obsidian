# Decoder-Only Transformer Knowledge Graph

```mermaid
graph TD

A[Tokenization]
B[Embeddings]

C[Input Matrix X]

D[Query Projection]
E[Key Projection]
F[Value Projection]

G[Q Matrix]
H[K Matrix]
I[V Matrix]

J[Attention Scores]

K[Causal Mask]

L[Softmax]

M[Attention Weights]

N[Attention Output]

O[Multi Head Attention]

P[Output Projection]

Q[Residual Connection]

R[LayerNorm]

S[Feed Forward Network]

T[Residual Connection]

U[LayerNorm]

V[Transformer Layer]

W[Stack Of Layers]

X[Final Hidden State]

Y[Logits]

Z[Softmax]

AA[Token Selection]

AB[Next Token]

A --> B
B --> C

C --> D
C --> E
C --> F

D --> G
E --> H
F --> I

G --> J
H --> J

J --> K
K --> L
L --> M

M --> N
I --> N

N --> O
O --> P

P --> Q
C --> Q

Q --> R

R --> S

S --> T
R --> T

T --> U

U --> V

V --> W

W --> X

X --> Y

Y --> Z

Z --> AA

AA --> AB
AB --> A
```

## Learning Order

1. [[01-Decoder-Only-Transformer-Overview]]
2. [[02-Tokenization]]
3. [[03-Embeddings]]
4. [[04-Matrix-Multiplication]]
5. [[05-Linear-Projections]]
6. [[06-Queries-Keys-Values]]
7. [[07-Self-Attention]]
8. [[08-Causal-Masking]]
9. [[09-Multi-Head-Attention]]
10. [[10-Residual-Connections]]
11. [[11-LayerNorm]]
12. [[12-FeedForward-Network]]
13. [[13-Transformer-Layer]]
14. [[14-Final-Hidden-State]]
15. [[15-Logits]]
16. [[16-Softmax]]
17. [[17-Token-Sampling]]