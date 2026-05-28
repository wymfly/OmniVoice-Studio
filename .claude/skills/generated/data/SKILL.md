---
name: data
description: "Skill for the Data area of OmniVoice-Studio. 16 symbols across 2 files."
---

# Data

16 symbols | 2 files | Cohesion: 100%

## When to Use

- Working with code in `omnivoice/`
- Understanding how load_audio_webdataset, should_continue, IterableDataReader work
- Modifying data-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `omnivoice/data/dataset.py` | IterableDataReader, WebDatasetReader, JsonlDatasetReader, MuxWebDatasetReader, WrappedIterableDataset (+7) |
| `omnivoice/data/batching.py` | StreamLengthGroupDataset, PackingIterableDataset, _get_bucket_id, __iter__ |

## Entry Points

Start here when exploring this area:

- **`load_audio_webdataset`** (Function) — `omnivoice/data/dataset.py:51`
- **`should_continue`** (Function) — `omnivoice/data/dataset.py:526`
- **`IterableDataReader`** (Class) — `omnivoice/data/dataset.py:281`
- **`WebDatasetReader`** (Class) — `omnivoice/data/dataset.py:306`
- **`JsonlDatasetReader`** (Class) — `omnivoice/data/dataset.py:361`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `IterableDataReader` | Class | `omnivoice/data/dataset.py` | 281 |
| `WebDatasetReader` | Class | `omnivoice/data/dataset.py` | 306 |
| `JsonlDatasetReader` | Class | `omnivoice/data/dataset.py` | 361 |
| `MuxWebDatasetReader` | Class | `omnivoice/data/dataset.py` | 450 |
| `WrappedIterableDataset` | Class | `omnivoice/data/dataset.py` | 296 |
| `StreamLengthGroupDataset` | Class | `omnivoice/data/batching.py` | 38 |
| `PackingIterableDataset` | Class | `omnivoice/data/batching.py` | 107 |
| `load_audio_webdataset` | Function | `omnivoice/data/dataset.py` | 51 |
| `should_continue` | Function | `omnivoice/data/dataset.py` | 526 |
| `_read_lines` | Method | `omnivoice/data/dataset.py` | 387 |
| `_stream_lines` | Method | `omnivoice/data/dataset.py` | 402 |
| `__iter__` | Method | `omnivoice/data/dataset.py` | 409 |
| `__call__` | Method | `omnivoice/data/dataset.py` | 221 |
| `__iter__` | Method | `omnivoice/data/dataset.py` | 520 |
| `_get_bucket_id` | Method | `omnivoice/data/batching.py` | 70 |
| `__iter__` | Method | `omnivoice/data/batching.py` | 74 |

## How to Explore

1. `gitnexus_context({name: "load_audio_webdataset"})` — see callers and callees
2. `gitnexus_query({query: "data"})` — find related execution flows
3. Read key files listed above for implementation details
