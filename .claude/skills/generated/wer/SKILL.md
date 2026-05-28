---
name: wer
description: "Skill for the Wer area of OmniVoice-Studio. 48 symbols across 11 files."
---

# Wer

48 symbols | 11 files | Cohesion: 89%

## When to Use

- Working with code in `omnivoice/`
- Understanding how read_test_list, get_parser, main work
- Modifying wer-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `omnivoice/eval/wer/minimax.py` | get_parser, main, __getitem__, run_eval_worker, run_eval_worker_paraformer (+6) |
| `omnivoice/eval/wer/sensevoice.py` | get_parser, main, run_eval_worker_sensevoice, post_process, load_sensevoice_model (+2) |
| `omnivoice/eval/wer/fleurs.py` | get_parser, main, run_eval_worker, clean_cjk_spaces, post_process (+2) |
| `omnivoice/eval/wer/seedtts.py` | get_parser, main, run_eval_worker, load_whisper_model, load_paraformer_model (+1) |
| `omnivoice/eval/wer/hubert.py` | get_parser, main, run_eval_worker, process_init, load_hubert_model |
| `omnivoice/eval/speaker_similarity/sim.py` | get_parser, main, get_embedding, run_similarity_worker |
| `omnivoice/eval/mos/utmos.py` | get_parser, main, run_utmos_worker |
| `omnivoice/eval/wer/common.py` | log_metrics, process_one |
| `omnivoice/utils/data_utils.py` | read_test_list |
| `omnivoice/eval/utils.py` | load_waveform |

## Entry Points

Start here when exploring this area:

- **`read_test_list`** (Function) — `omnivoice/utils/data_utils.py:28`
- **`get_parser`** (Function) — `omnivoice/eval/wer/seedtts.py:45`
- **`main`** (Function) — `omnivoice/eval/wer/seedtts.py:281`
- **`get_parser`** (Function) — `omnivoice/eval/wer/hubert.py:42`
- **`main`** (Function) — `omnivoice/eval/wer/hubert.py:198`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `read_test_list` | Function | `omnivoice/utils/data_utils.py` | 28 |
| `get_parser` | Function | `omnivoice/eval/wer/seedtts.py` | 45 |
| `main` | Function | `omnivoice/eval/wer/seedtts.py` | 281 |
| `get_parser` | Function | `omnivoice/eval/wer/hubert.py` | 42 |
| `main` | Function | `omnivoice/eval/wer/hubert.py` | 198 |
| `get_parser` | Function | `omnivoice/eval/speaker_similarity/sim.py` | 46 |
| `main` | Function | `omnivoice/eval/speaker_similarity/sim.py` | 182 |
| `get_parser` | Function | `omnivoice/eval/mos/utmos.py` | 45 |
| `main` | Function | `omnivoice/eval/mos/utmos.py` | 158 |
| `get_parser` | Function | `omnivoice/eval/wer/sensevoice.py` | 44 |
| `main` | Function | `omnivoice/eval/wer/sensevoice.py` | 229 |
| `get_parser` | Function | `omnivoice/eval/wer/minimax.py` | 65 |
| `main` | Function | `omnivoice/eval/wer/minimax.py` | 371 |
| `get_parser` | Function | `omnivoice/eval/wer/fleurs.py` | 147 |
| `main` | Function | `omnivoice/eval/wer/fleurs.py` | 326 |
| `log_metrics` | Function | `omnivoice/eval/wer/common.py` | 67 |
| `load_waveform` | Function | `omnivoice/eval/utils.py` | 25 |
| `run_eval_worker` | Function | `omnivoice/eval/wer/hubert.py` | 158 |
| `get_embedding` | Function | `omnivoice/eval/speaker_similarity/sim.py` | 144 |
| `run_similarity_worker` | Function | `omnivoice/eval/speaker_similarity/sim.py` | 150 |

## How to Explore

1. `gitnexus_context({name: "read_test_list"})` — see callers and callees
2. `gitnexus_query({query: "wer"})` — find related execution flows
3. Read key files listed above for implementation details
