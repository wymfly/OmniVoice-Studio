---
name: omnivoice-gguf
description: "Skill for the Omnivoice_gguf area of OmniVoice-Studio. 26 symbols across 4 files."
---

# Omnivoice_gguf

26 symbols | 4 files | Cohesion: 95%

## When to Use

- Working with code in `backend/`
- Understanding how set_quant_override, test_bucket_thresholds_directly, detect_capabilities work
- Modifying omnivoice_gguf-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `backend/engines/omnivoice_gguf/backend.py` | _mask_token, _load_quant_map, _walk_quant_entries, _allowed_quant_filenames, _ensure_quant_map (+17) |
| `backend/engines/omnivoice_gguf/hardware_probe.py` | _bucket, detect_capabilities |
| `backend/services/settings_store.py` | set_quant_override |
| `tests/backend/engines/test_hardware_probe.py` | test_bucket_thresholds_directly |

## Entry Points

Start here when exploring this area:

- **`set_quant_override`** (Function) — `backend/services/settings_store.py:194`
- **`test_bucket_thresholds_directly`** (Function) — `tests/backend/engines/test_hardware_probe.py:107`
- **`detect_capabilities`** (Function) — `backend/engines/omnivoice_gguf/hardware_probe.py:71`
- **`select_default_engine`** (Function) — `backend/engines/omnivoice_gguf/backend.py:680`
- **`generate`** (Method) — `backend/engines/omnivoice_gguf/backend.py:487`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `set_quant_override` | Function | `backend/services/settings_store.py` | 194 |
| `test_bucket_thresholds_directly` | Function | `tests/backend/engines/test_hardware_probe.py` | 107 |
| `detect_capabilities` | Function | `backend/engines/omnivoice_gguf/hardware_probe.py` | 71 |
| `select_default_engine` | Function | `backend/engines/omnivoice_gguf/backend.py` | 680 |
| `generate` | Method | `backend/engines/omnivoice_gguf/backend.py` | 487 |
| `is_available` | Method | `backend/engines/omnivoice_gguf/backend.py` | 319 |
| `probe_load` | Method | `backend/engines/omnivoice_gguf/backend.py` | 446 |
| `_bucket` | Function | `backend/engines/omnivoice_gguf/hardware_probe.py` | 53 |
| `_mask_token` | Function | `backend/engines/omnivoice_gguf/backend.py` | 83 |
| `_load_quant_map` | Function | `backend/engines/omnivoice_gguf/backend.py` | 121 |
| `_walk_quant_entries` | Function | `backend/engines/omnivoice_gguf/backend.py` | 146 |
| `_allowed_quant_filenames` | Function | `backend/engines/omnivoice_gguf/backend.py` | 166 |
| `_platform_slug` | Function | `backend/engines/omnivoice_gguf/backend.py` | 89 |
| `_binary_path` | Function | `backend/engines/omnivoice_gguf/backend.py` | 112 |
| `_sha256_of_file` | Function | `backend/engines/omnivoice_gguf/backend.py` | 184 |
| `_load_checksum_manifest` | Function | `backend/engines/omnivoice_gguf/backend.py` | 192 |
| `_is_macos_quarantined` | Function | `backend/engines/omnivoice_gguf/backend.py` | 224 |
| `_iso_to_omnivoice_lang` | Function | `backend/engines/omnivoice_gguf/backend.py` | 634 |
| `_import_tts_backend` | Function | `backend/engines/omnivoice_gguf/backend.py` | 252 |
| `_make_backend_class` | Function | `backend/engines/omnivoice_gguf/backend.py` | 271 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Generate → _load_quant_map` | intra_community | 5 |
| `Generate → _walk_quant_entries` | intra_community | 5 |
| `Generate → _bucket` | intra_community | 5 |
| `Generate → _platform_slug` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Routers | 1 calls |

## How to Explore

1. `gitnexus_context({name: "set_quant_override"})` — see callers and callees
2. `gitnexus_query({query: "omnivoice_gguf"})` — find related execution flows
3. Read key files listed above for implementation details
