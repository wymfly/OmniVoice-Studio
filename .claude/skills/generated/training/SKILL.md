---
name: training
description: "Skill for the Training area of OmniVoice-Studio. 18 symbols across 6 files."
---

# Training

18 symbols | 6 files | Cohesion: 89%

## When to Use

- Working with code in `omnivoice/`
- Understanding how save_checkpoint, build_model_and_tokenizer, build_dataloaders work
- Modifying training-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `omnivoice/training/trainer.py` | _to_device, save_checkpoint, load_checkpoint, evaluate, train (+3) |
| `omnivoice/training/checkpoint.py` | update, log_metrics, close, save_checkpoint |
| `omnivoice/training/builder.py` | build_model_and_tokenizer, build_dataloaders |
| `omnivoice/data/dataset.py` | prepare_data_manifests_from_json, webdataset_manifest_reader |
| `omnivoice/training/config.py` | from_json |
| `omnivoice/cli/train.py` | main |

## Entry Points

Start here when exploring this area:

- **`save_checkpoint`** (Function) — `omnivoice/training/checkpoint.py:117`
- **`build_model_and_tokenizer`** (Function) — `omnivoice/training/builder.py:48`
- **`build_dataloaders`** (Function) — `omnivoice/training/builder.py:122`
- **`prepare_data_manifests_from_json`** (Function) — `omnivoice/data/dataset.py:65`
- **`webdataset_manifest_reader`** (Function) — `omnivoice/data/dataset.py:160`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `save_checkpoint` | Function | `omnivoice/training/checkpoint.py` | 117 |
| `build_model_and_tokenizer` | Function | `omnivoice/training/builder.py` | 48 |
| `build_dataloaders` | Function | `omnivoice/training/builder.py` | 122 |
| `prepare_data_manifests_from_json` | Function | `omnivoice/data/dataset.py` | 65 |
| `webdataset_manifest_reader` | Function | `omnivoice/data/dataset.py` | 160 |
| `main` | Function | `omnivoice/cli/train.py` | 39 |
| `save_checkpoint` | Method | `omnivoice/training/trainer.py` | 186 |
| `load_checkpoint` | Method | `omnivoice/training/trainer.py` | 201 |
| `evaluate` | Method | `omnivoice/training/trainer.py` | 208 |
| `train` | Method | `omnivoice/training/trainer.py` | 242 |
| `update` | Method | `omnivoice/training/checkpoint.py` | 65 |
| `log_metrics` | Method | `omnivoice/training/checkpoint.py` | 84 |
| `close` | Method | `omnivoice/training/checkpoint.py` | 112 |
| `from_json` | Method | `omnivoice/training/config.py` | 86 |
| `create_optimizer_and_scheduler` | Method | `omnivoice/training/trainer.py` | 160 |
| `_to_device` | Function | `omnivoice/training/trainer.py` | 47 |
| `__init__` | Method | `omnivoice/training/trainer.py` | 56 |
| `_init_accelerator` | Method | `omnivoice/training/trainer.py` | 98 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Main → Webdataset_manifest_reader` | intra_community | 4 |
| `Main → Load_checkpoint` | cross_community | 3 |
| `Main → Start` | cross_community | 3 |
| `Main → Update` | cross_community | 3 |
| `Main → Log_metrics` | cross_community | 3 |
| `Main → From_pretrained` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Hooks | 1 calls |
| Cli | 1 calls |

## How to Explore

1. `gitnexus_context({name: "save_checkpoint"})` — see callers and callees
2. `gitnexus_query({query: "training"})` — find related execution flows
3. Read key files listed above for implementation details
