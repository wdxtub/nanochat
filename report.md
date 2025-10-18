# nanochat training report

Generated: 2025-10-19 07:18:17

## Environment

### Git Information
- Branch: cpu-mps-dev
- Commit: cf2baf9 (dirty)
- Message: fix typo

### Hardware
- Platform: Darwin
- CPUs: 14 cores (14 logical)
- Memory: 36.0 GB
- GPUs: None available

### Software
- Python: 3.10.17
- PyTorch: 2.9.0


### Bloat
- Characters: 355,952
- Lines: 8,686
- Files: 45
- Tokens (approx): 88,988
- Dependencies (uv.lock lines): 2,032

Run started: 2025-10-19 07:18:17

---

## Tokenizer training
timestamp: 2025-10-19 07:19:21

- max_chars: 2,000,000,000
- doc_cap: 10,000
- vocab_size: 65,536
- train_time: 54.3550
- num_special_tokens: 9
- token_bytes_min: 1
- token_bytes_max: 32
- token_bytes_mean: 6.9151
- token_bytes_std: 2.8736


## Tokenizer evaluation
timestamp: 2025-10-19 07:19:24

### Comparison with GPT-2

| Text Type | Bytes | GPT-2 Tokens | GPT-2 Ratio | Ours Tokens | Ours Ratio | Relative Diff % |
|-----------|-------|--------------|--------------|-------------|------------|-----------------|
| news | 1819 | 404 | 4.50 | 375 | 4.85 | +7.2% |
| korean | 893 | 745 | 1.20 | 721 | 1.24 | +3.2% |
| code | 1259 | 576 | 2.19 | 493 | 2.55 | +14.4% |
| math | 1834 | 936 | 1.96 | 966 | 1.90 | -3.2% |
| science | 1112 | 260 | 4.28 | 225 | 4.94 | +13.5% |
| fwe-train | 4208518 | 900364 | 4.67 | 856901 | 4.91 | +4.8% |
| fwe-val | 4908443 | 1059062 | 4.63 | 1010356 | 4.86 | +4.6% |

### Comparison with GPT-4

| Text Type | Bytes | GPT-4 Tokens | GPT-4 Ratio | Ours Tokens | Ours Ratio | Relative Diff % |
|-----------|-------|--------------|--------------|-------------|------------|-----------------|
| news | 1819 | 387 | 4.70 | 375 | 4.85 | +3.1% |
| korean | 893 | 364 | 2.45 | 721 | 1.24 | -98.1% |
| code | 1259 | 309 | 4.07 | 493 | 2.55 | -59.5% |
| math | 1834 | 832 | 2.20 | 966 | 1.90 | -16.1% |
| science | 1112 | 249 | 4.47 | 225 | 4.94 | +9.6% |
| fwe-train | 4208518 | 874799 | 4.81 | 856901 | 4.91 | +2.0% |
| fwe-val | 4908443 | 1029691 | 4.77 | 1010356 | 4.86 | +1.9% |


## Summary

- Characters: 355,952
- Lines: 8,686
- Files: 45
- Tokens (approx): 88,988
- Dependencies (uv.lock lines): 2,032

| Metric          | BASE     | MID      | SFT      | RL       |
|-----------------|----------|----------|----------|----------|

Total wall clock time: 0h1m
