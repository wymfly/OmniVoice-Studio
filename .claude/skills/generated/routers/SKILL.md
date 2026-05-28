---
name: routers
description: "Skill for the Routers area of OmniVoice-Studio. 165 symbols across 39 files."
---

# Routers

165 symbols | 39 files | Cohesion: 85%

## When to Use

- Working with code in `backend/`
- Understanding how get_hf_token, set_hf_token, clear_hf_token work
- Modifying routers-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `backend/api/routers/dub_export.py` | _unique_stamp, _native_save, _ffmpeg_filter_escape, dub_download, dub_preview_video (+11) |
| `backend/api/routers/system.py` | clean_audio, _do_clean_audio, _has_hf_token, loaded_models, system_info (+6) |
| `backend/api/routers/profiles.py` | list_profiles, create_profile, get_profile, update_profile, get_profile_usage (+5) |
| `backend/api/routers/gallery.py` | list_voices, get_voice, delete_voice, download_youtube_clip, upload_voice_clip (+5) |
| `backend/api/routers/dub_core.py` | list_dub_history, clear_dub_history, delete_single_dub_history, preview_upload, _transcribe_chunk (+3) |
| `backend/api/routers/glossary.py` | add_term, delete_term, clear_terms, _row_to_dict, list_terms (+2) |
| `backend/api/routers/capture_ws.py` | _run, ws_transcribe, receive_audio, _safe_send, process_partials (+2) |
| `backend/api/routers/settings.py` | _state_response, save_hf_token, clear_hf_token, get_hf_token_state, _torch_compile_state (+2) |
| `backend/core/job_store.py` | create, append_event, events_since, get, list_jobs (+1) |
| `backend/api/routers/openai_compat.py` | create_transcription, _format_ts_srt, _format_ts_vtt, _resolve_engine, _encode_audio (+1) |

## Entry Points

Start here when exploring this area:

- **`get_hf_token`** (Function) — `backend/services/settings_store.py:36`
- **`set_hf_token`** (Function) — `backend/services/settings_store.py:75`
- **`clear_hf_token`** (Function) — `backend/services/settings_store.py:100`
- **`get_job`** (Function) — `backend/services/dub_pipeline.py:179`
- **`derive_fernet_key`** (Function) — `backend/services/_secret_key.py:137`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `get_hf_token` | Function | `backend/services/settings_store.py` | 36 |
| `set_hf_token` | Function | `backend/services/settings_store.py` | 75 |
| `clear_hf_token` | Function | `backend/services/settings_store.py` | 100 |
| `get_job` | Function | `backend/services/dub_pipeline.py` | 179 |
| `derive_fernet_key` | Function | `backend/services/_secret_key.py` | 137 |
| `create` | Function | `backend/core/job_store.py` | 37 |
| `append_event` | Function | `backend/core/job_store.py` | 82 |
| `events_since` | Function | `backend/core/job_store.py` | 113 |
| `get` | Function | `backend/core/job_store.py` | 127 |
| `list_jobs` | Function | `backend/core/job_store.py` | 133 |
| `sweep_orphans_on_startup` | Function | `backend/core/job_store.py` | 158 |
| `db_conn` | Function | `backend/core/db.py` | 21 |
| `list_projects` | Function | `backend/api/routers/projects.py` | 12 |
| `get_project` | Function | `backend/api/routers/projects.py` | 20 |
| `create_project` | Function | `backend/api/routers/projects.py` | 36 |
| `update_project` | Function | `backend/api/routers/projects.py` | 48 |
| `delete_project` | Function | `backend/api/routers/projects.py` | 62 |
| `list_profiles` | Function | `backend/api/routers/profiles.py` | 31 |
| `create_profile` | Function | `backend/api/routers/profiles.py` | 37 |
| `get_profile` | Function | `backend/api/routers/profiles.py` | 69 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Enqueue_batch_job → _lazy_torch` | cross_community | 9 |
| `Export_file → _load` | cross_community | 6 |
| `Ws_tts → _lazy_torch` | cross_community | 6 |
| `Dub_generate → _lazy_torch` | cross_community | 6 |
| `Get_hf_token → Get_db` | cross_community | 6 |
| `Set_hf_token → Get_db` | cross_community | 6 |
| `Enqueue_batch_job → _safe_torchaudio_save` | cross_community | 6 |
| `Create_transcription → Is_available` | cross_community | 5 |
| `Create_transcription → Is_available` | cross_community | 5 |
| `Create_transcription → Is_available` | cross_community | 5 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Services | 14 calls |
| Tests | 3 calls |
| Cluster_174 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "get_hf_token"})` — see callers and callees
2. `gitnexus_query({query: "routers"})` — find related execution flows
3. Read key files listed above for implementation details
