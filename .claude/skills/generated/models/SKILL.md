---
name: models
description: "Skill for the Models area of OmniVoice-Studio. 46 symbols across 5 files."
---

# Models

46 symbols | 5 files | Cohesion: 83%

## When to Use

- Working with code in `omnivoice/`
- Understanding how add_punctuation, remove_silence, remove_silence_edges work
- Modifying models-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `omnivoice/models/omnivoice.py` | transcribe, create_voice_clone_prompt, _prepare_inference_inputs, _generate_iterative, _predict_tokens_with_scoring (+22) |
| `omnivoice/utils/audio.py` | remove_silence, remove_silence_edges, audiosegment_to_tensor, tensor_to_audiosegment, trim_long_audio (+2) |
| `omnivoice/eval/models/utmos.py` | __init__, block, build_encoder_layer, __init__, forward (+1) |
| `omnivoice/eval/models/ecapa_tdnn_wavlm.py` | __init__, get_feat_num, get_feat, forward |
| `omnivoice/utils/text.py` | add_punctuation, chunk_text_punctuation |

## Entry Points

Start here when exploring this area:

- **`add_punctuation`** (Function) — `omnivoice/utils/text.py:206`
- **`remove_silence`** (Function) — `omnivoice/utils/audio.py:69`
- **`remove_silence_edges`** (Function) — `omnivoice/utils/audio.py:116`
- **`audiosegment_to_tensor`** (Function) — `omnivoice/utils/audio.py:149`
- **`tensor_to_audiosegment`** (Function) — `omnivoice/utils/audio.py:169`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `add_punctuation` | Function | `omnivoice/utils/text.py` | 206 |
| `remove_silence` | Function | `omnivoice/utils/audio.py` | 69 |
| `remove_silence_edges` | Function | `omnivoice/utils/audio.py` | 116 |
| `audiosegment_to_tensor` | Function | `omnivoice/utils/audio.py` | 149 |
| `tensor_to_audiosegment` | Function | `omnivoice/utils/audio.py` | 169 |
| `trim_long_audio` | Function | `omnivoice/utils/audio.py` | 257 |
| `chunk_text_punctuation` | Function | `omnivoice/utils/text.py` | 118 |
| `fade_and_pad_audio` | Function | `omnivoice/utils/audio.py` | 205 |
| `cross_fade_chunks` | Function | `omnivoice/utils/audio.py` | 307 |
| `block` | Function | `omnivoice/eval/models/utmos.py` | 138 |
| `pad_to_multiple` | Function | `omnivoice/eval/models/utmos.py` | 251 |
| `transcribe` | Method | `omnivoice/models/omnivoice.py` | 326 |
| `create_voice_clone_prompt` | Method | `omnivoice/models/omnivoice.py` | 598 |
| `from_dict` | Method | `omnivoice/models/omnivoice.py` | 104 |
| `get_indices` | Method | `omnivoice/models/omnivoice.py` | 122 |
| `slice_task` | Method | `omnivoice/models/omnivoice.py` | 128 |
| `generate` | Method | `omnivoice/models/omnivoice.py` | 473 |
| `get_input_embeddings` | Method | `omnivoice/models/omnivoice.py` | 357 |
| `forward` | Method | `omnivoice/models/omnivoice.py` | 385 |
| `build_encoder_layer` | Method | `omnivoice/eval/models/utmos.py` | 175 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Generate → _ensure_list` | cross_community | 3 |
| `Create_voice_clone_prompt → Tensor_to_audiosegment` | intra_community | 3 |
| `Create_voice_clone_prompt → Audiosegment_to_tensor` | intra_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Cli | 2 calls |

## How to Explore

1. `gitnexus_context({name: "add_punctuation"})` — see callers and callees
2. `gitnexus_query({query: "models"})` — find related execution flows
3. Read key files listed above for implementation details
