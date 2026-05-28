---
name: setup
description: "Skill for the Setup area of OmniVoice-Studio. 27 symbols across 5 files."
---

# Setup

27 symbols | 5 files | Cohesion: 87%

## When to Use

- Working with code in `backend/`
- Understanding how resolve_ffprobe, find_ffprobe, probe work
- Modifying setup-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `backend/api/routers/setup/models.py` | supported_on_host, _current_platform_tags, _model_supported, _cached, _set_cache (+8) |
| `backend/api/routers/setup/wizard.py` | _run_cmd, _detect_gpu, _probe_network, _ram_gb, preflight (+2) |
| `backend/api/routers/setup/download.py` | _do, delete_model, setup_download_stream, gen |
| `backend/services/ffmpeg_utils.py` | resolve_ffprobe, find_ffprobe |
| `backend/api/routers/tools.py` | probe |

## Entry Points

Start here when exploring this area:

- **`resolve_ffprobe`** (Function) — `backend/services/ffmpeg_utils.py:53`
- **`find_ffprobe`** (Function) — `backend/services/ffmpeg_utils.py:85`
- **`probe`** (Function) — `backend/api/routers/tools.py:43`
- **`preflight`** (Function) — `backend/api/routers/setup/wizard.py:202`
- **`list_models`** (Function) — `backend/api/routers/setup/models.py:168`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `resolve_ffprobe` | Function | `backend/services/ffmpeg_utils.py` | 53 |
| `find_ffprobe` | Function | `backend/services/ffmpeg_utils.py` | 85 |
| `probe` | Function | `backend/api/routers/tools.py` | 43 |
| `preflight` | Function | `backend/api/routers/setup/wizard.py` | 202 |
| `list_models` | Function | `backend/api/routers/setup/models.py` | 168 |
| `setup_status` | Function | `backend/api/routers/setup/wizard.py` | 52 |
| `hf_cache_dir` | Function | `backend/api/routers/setup/models.py` | 117 |
| `is_cached` | Function | `backend/api/routers/setup/models.py` | 126 |
| `invalidate_cache` | Function | `backend/api/routers/setup/models.py` | 160 |
| `delete_model` | Function | `backend/api/routers/setup/download.py` | 211 |
| `recommendations` | Function | `backend/api/routers/setup/models.py` | 212 |
| `setup_download_stream` | Function | `backend/api/routers/setup/download.py` | 45 |
| `gen` | Function | `backend/api/routers/setup/download.py` | 58 |
| `supported_on_host` | Method | `backend/api/routers/setup/models.py` | 78 |
| `get` | Method | `backend/api/routers/setup/models.py` | 67 |
| `all` | Method | `backend/api/routers/setup/models.py` | 75 |
| `_run_cmd` | Function | `backend/api/routers/setup/wizard.py` | 78 |
| `_detect_gpu` | Function | `backend/api/routers/setup/wizard.py` | 90 |
| `_probe_network` | Function | `backend/api/routers/setup/wizard.py` | 183 |
| `_ram_gb` | Function | `backend/api/routers/setup/wizard.py` | 193 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `List_models → _current_platform_tags` | intra_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Routers | 2 calls |

## How to Explore

1. `gitnexus_context({name: "resolve_ffprobe"})` — see callers and callees
2. `gitnexus_query({query: "setup"})` — find related execution flows
3. Read key files listed above for implementation details
