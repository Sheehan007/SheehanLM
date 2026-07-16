# SheehanLM

# Project Descpription 

-- WILL UPDATE -- 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### File-management rules 
1. src/ contains reusable implementation
2. scripts/ contains thin commands that call functionality from src/
3. configs/ contains choices and hyperparameters, not Python code
4. tests/ mirrors the structure of src/
5. docs/decisions/ records why I selected an architectural choice
6. data/, runs/ and checkpoints/ stay out of normal Git history

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Shared conventions
1. B - batch size
2. T - sequence length
3. V - vocabulary size
4. C - model width
5. L - no. of transformer layers
6. H - no. of query heads
7. Hkv - no. of key/value heads
8. Dh - head dimension
9. F - feed-forward hidden dimension

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### For SheehanLM-42M: 
1. V   = 16,384
2. C   = 512
3. L   = 12
4. H   = 8
5. Hkv = 2
6. Dh  = 64
7. F   = 1,408
8. T   = 1,024 initially

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Main shapes
1. token IDs:       [B, T]
2. embeddings:      [B, T, C]
3. queries:         [B, H, T, Dh]
4. keys/values:     [B, Hkv, T, Dh]
5. attention:       [B, H, T, T]
6. hidden states:   [B, T, C]
7. logits:          [B, T, V]

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Day-wise progress

Day-1: wrote the config.py for my 350M model 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Project Phases

**Phase-1** - Building the Transformer

















