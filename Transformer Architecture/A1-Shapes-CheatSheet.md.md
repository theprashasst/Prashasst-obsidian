# Shapes Cheat Sheet

| Tensor | Shape |
|----------|----------|
| Input IDs | N |
| Embeddings X | N × D |
| Q | N × Dh |
| K | N × Dh |
| V | N × Dh |
| Scores | N × N |
| Attention Weights | N × N |
| Attention Output | N × Dh |
| MHA Output | N × D |
| FFN Hidden | N × 4D |
| FFN Output | N × D |
| Final Hidden | N × D |
| Logits | 1 × Vocab |
