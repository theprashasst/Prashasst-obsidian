

## Complete Pipeline

Input Text

↓

[[02-Tokenization]]

↓

[[03-Embeddings]]

↓

[[06-Queries-Keys-Values]]

↓

[[07-Self-Attention]]

↓

[[08-Causal-Masking]]

↓

[[09-Multi-Head-Attention]]

↓

[[10-Residual-Connections]]

↓

[[11-LayerNorm]]

↓

[[12-FeedForward-Network]]

↓

Repeat For Many Layers

↓

[[14-Final-Hidden-State]]

↓

[[15-Logits]]

↓

[[16-Softmax]]

↓

[[17-Token-Sampling]]

↓

Next Token

---

## Typical GPT Dimensions

| Parameter | GPT Style |
|------------|------------|
| Layers | 80 |
| Hidden Size D | 4096 |
| Heads | 32 |
| Head Dim Dh | 128 |
| Vocabulary | 50k-100k |

Relationship:

```text
D = H × Dh

4096 = 32 × 128
```