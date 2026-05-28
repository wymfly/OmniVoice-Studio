---
name: cli
description: "Skill for the Cli area of OmniVoice-Studio. 28 symbols across 7 files."
---

# Cli

28 symbols | 7 files | Cohesion: 93%

## When to Use

- Working with code in `omnivoice/`
- Understanding how load_audio, get_best_device, get_parser work
- Modifying cli-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `omnivoice/cli/demo.py` | get_best_device, build_parser, build_demo, _lang_dropdown, _gen_settings (+3) |
| `omnivoice/cli/infer_batch.py` | get_best_device, get_parser, estimate_sample_total_duration, cluster_samples_by_duration, cluster_samples_by_batch_size (+2) |
| `omnivoice/cli/dub.py` | _log, _post, _stream_task, main |
| `omnivoice/utils/duration.py` | _get_char_weight, calculate_total_weight, estimate_duration |
| `omnivoice/cli/infer.py` | get_best_device, get_parser, main |
| `omnivoice/models/omnivoice.py` | from_pretrained, load_asr_model |
| `omnivoice/utils/audio.py` | load_audio |

## Entry Points

Start here when exploring this area:

- **`load_audio`** (Function) — `omnivoice/utils/audio.py:31`
- **`get_best_device`** (Function) — `omnivoice/cli/infer_batch.py:54`
- **`get_parser`** (Function) — `omnivoice/cli/infer_batch.py:67`
- **`estimate_sample_total_duration`** (Function) — `omnivoice/cli/infer_batch.py:254`
- **`cluster_samples_by_duration`** (Function) — `omnivoice/cli/infer_batch.py:273`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `load_audio` | Function | `omnivoice/utils/audio.py` | 31 |
| `get_best_device` | Function | `omnivoice/cli/infer_batch.py` | 54 |
| `get_parser` | Function | `omnivoice/cli/infer_batch.py` | 67 |
| `estimate_sample_total_duration` | Function | `omnivoice/cli/infer_batch.py` | 254 |
| `cluster_samples_by_duration` | Function | `omnivoice/cli/infer_batch.py` | 273 |
| `cluster_samples_by_batch_size` | Function | `omnivoice/cli/infer_batch.py` | 315 |
| `main` | Function | `omnivoice/cli/infer_batch.py` | 404 |
| `process_init` | Function | `omnivoice/cli/infer_batch.py` | 202 |
| `get_best_device` | Function | `omnivoice/cli/infer.py` | 31 |
| `get_parser` | Function | `omnivoice/cli/infer.py` | 40 |
| `main` | Function | `omnivoice/cli/infer.py` | 120 |
| `get_best_device` | Function | `omnivoice/cli/demo.py` | 37 |
| `build_parser` | Function | `omnivoice/cli/demo.py` | 112 |
| `build_demo` | Function | `omnivoice/cli/demo.py` | 153 |
| `main` | Function | `omnivoice/cli/demo.py` | 506 |
| `main` | Function | `omnivoice/cli/dub.py` | 109 |
| `calculate_total_weight` | Method | `omnivoice/utils/duration.py` | 203 |
| `estimate_duration` | Method | `omnivoice/utils/duration.py` | 207 |
| `from_pretrained` | Method | `omnivoice/models/omnivoice.py` | 245 |
| `load_asr_model` | Method | `omnivoice/models/omnivoice.py` | 305 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Main → _get_char_weight` | intra_community | 6 |
| `Main → Load_audio` | intra_community | 4 |
| `Main → From_pretrained` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Wer | 1 calls |

## How to Explore

1. `gitnexus_context({name: "load_audio"})` — see callers and callees
2. `gitnexus_query({query: "cli"})` — find related execution flows
3. Read key files listed above for implementation details
