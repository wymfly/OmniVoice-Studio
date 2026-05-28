---
name: indextts
description: "Skill for the Indextts area of OmniVoice-Studio. 12 symbols across 3 files."
---

# Indextts

12 symbols | 3 files | Cohesion: 97%

## When to Use

- Working with code in `backend/`
- Understanding how main, resolve_indextts_venv, venv_python work
- Modifying indextts-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `backend/engines/indextts/main.py` | _send, _recv, _load_model, _wav_to_pcm_b64, _handle_synthesize (+1) |
| `backend/engines/indextts/bootstrap.py` | resolve_indextts_venv, _venv_python_path, _venv_can_import_indextts, _locate_uv, _bootstrap_engines_venv |
| `backend/engines/indextts/__init__.py` | venv_python |

## Entry Points

Start here when exploring this area:

- **`main`** (Function) — `backend/engines/indextts/main.py:250`
- **`resolve_indextts_venv`** (Function) — `backend/engines/indextts/bootstrap.py:96`
- **`venv_python`** (Method) — `backend/engines/indextts/__init__.py:109`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `main` | Function | `backend/engines/indextts/main.py` | 250 |
| `resolve_indextts_venv` | Function | `backend/engines/indextts/bootstrap.py` | 96 |
| `venv_python` | Method | `backend/engines/indextts/__init__.py` | 109 |
| `_send` | Function | `backend/engines/indextts/main.py` | 99 |
| `_recv` | Function | `backend/engines/indextts/main.py` | 106 |
| `_load_model` | Function | `backend/engines/indextts/main.py` | 130 |
| `_wav_to_pcm_b64` | Function | `backend/engines/indextts/main.py` | 167 |
| `_handle_synthesize` | Function | `backend/engines/indextts/main.py` | 197 |
| `_venv_python_path` | Function | `backend/engines/indextts/bootstrap.py` | 143 |
| `_venv_can_import_indextts` | Function | `backend/engines/indextts/bootstrap.py` | 164 |
| `_locate_uv` | Function | `backend/engines/indextts/bootstrap.py` | 190 |
| `_bootstrap_engines_venv` | Function | `backend/engines/indextts/bootstrap.py` | 201 |

## How to Explore

1. `gitnexus_context({name: "main"})` — see callers and callees
2. `gitnexus_query({query: "indextts"})` — find related execution flows
3. Read key files listed above for implementation details
