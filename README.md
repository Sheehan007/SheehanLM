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
V   = 16,384
C   = 512
L   = 12
H   = 8
Hkv = 2
Dh  = 64
F   = 1,408
T   = 1,024 initially















