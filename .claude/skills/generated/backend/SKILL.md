---
name: backend
description: "Skill for the Backend area of OmniVoice-Studio. 34 symbols across 8 files."
---

# Backend

34 symbols | 8 files | Cohesion: 93%

## When to Use

- Working with code in `backend/`
- Understanding how generate_speech, list_voices, list_personalities work
- Modifying backend-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `backend/mcp_server.py` | _api_base, _api_get, _api_post_form, generate_speech, list_voices (+7) |
| `tests/backend/test_engine_spawn_token.py` | _client, test_post_hf_token_loopback_succeeds, test_delete_hf_token_clears_store, test_get_hf_token_state_returns_three_rows, _build_subprocess_env (+2) |
| `backend/main.py` | _env_flag, lifespan, _preload_capture_asr, format |
| `tests/backend/test_perf_settings.py` | _client, test_get_default_state, test_put_enabled_true_persists, test_value_round_trips_via_settings_store |
| `tests/backend/test_dub_pipeline_wav.py` | _bare_audio_writes_in_routers, test_no_bare_audio_writes_in_routers, test_no_bare_audio_writes_via_subprocess_grep, _which |
| `backend/api/http_client.py` | close_http_client |
| `backend/api/routers/gallery.py` | _init_gallery_db |
| `frontend/src/ui/Slider.jsx` | Slider |

## Entry Points

Start here when exploring this area:

- **`generate_speech`** (Function) — `backend/mcp_server.py:79`
- **`list_voices`** (Function) — `backend/mcp_server.py:129`
- **`list_personalities`** (Function) — `backend/mcp_server.py:139`
- **`check_health`** (Function) — `backend/mcp_server.py:163`
- **`get_voice`** (Function) — `backend/mcp_server.py:171`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `generate_speech` | Function | `backend/mcp_server.py` | 79 |
| `list_voices` | Function | `backend/mcp_server.py` | 129 |
| `list_personalities` | Function | `backend/mcp_server.py` | 139 |
| `check_health` | Function | `backend/mcp_server.py` | 163 |
| `get_voice` | Function | `backend/mcp_server.py` | 171 |
| `get_recent_history` | Function | `backend/mcp_server.py` | 180 |
| `lifespan` | Function | `backend/main.py` | 251 |
| `close_http_client` | Function | `backend/api/http_client.py` | 36 |
| `test_get_default_state` | Function | `tests/backend/test_perf_settings.py` | 49 |
| `test_put_enabled_true_persists` | Function | `tests/backend/test_perf_settings.py` | 61 |
| `test_value_round_trips_via_settings_store` | Function | `tests/backend/test_perf_settings.py` | 86 |
| `test_post_hf_token_loopback_succeeds` | Function | `tests/backend/test_engine_spawn_token.py` | 52 |
| `test_delete_hf_token_clears_store` | Function | `tests/backend/test_engine_spawn_token.py` | 88 |
| `test_get_hf_token_state_returns_three_rows` | Function | `tests/backend/test_engine_spawn_token.py` | 112 |
| `create_mcp_server` | Function | `backend/mcp_server.py` | 45 |
| `main` | Function | `backend/mcp_server.py` | 190 |
| `test_subprocess_env_includes_hf_token_when_resolved` | Function | `tests/backend/test_engine_spawn_token.py` | 159 |
| `test_subprocess_env_unchanged_when_no_token` | Function | `tests/backend/test_engine_spawn_token.py` | 186 |
| `test_no_bare_audio_writes_in_routers` | Function | `tests/backend/test_dub_pipeline_wav.py` | 79 |
| `test_no_bare_audio_writes_via_subprocess_grep` | Function | `tests/backend/test_dub_pipeline_wav.py` | 95 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Lifespan → _add_column_if_missing` | cross_community | 4 |
| `Lifespan → Get_db` | cross_community | 4 |
| `Lifespan → _init_queue` | cross_community | 3 |
| `Lifespan → _push_event` | cross_community | 3 |
| `Lifespan → _lazy_torch` | cross_community | 3 |
| `Lifespan → _run_alembic_upgrade` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Services | 3 calls |
| Cluster_177 | 2 calls |
| Tests | 1 calls |
| Routers | 1 calls |

## How to Explore

1. `gitnexus_context({name: "generate_speech"})` — see callers and callees
2. `gitnexus_query({query: "backend"})` — find related execution flows
3. Read key files listed above for implementation details
