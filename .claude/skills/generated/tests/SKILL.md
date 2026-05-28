---
name: tests
description: "Skill for the Tests area of OmniVoice-Studio. 141 symbols across 28 files."
---

# Tests

141 symbols | 28 files | Cohesion: 92%

## When to Use

- Working with code in `tests/`
- Understanding how test_atomic_save_wav_assembly_pattern, atomic_save_wav, test_atomic_save_wav_delegates_to_safe_helper work
- Modifying tests-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `backend/tests/test_batch.py` | _enqueue, test_returns_job_id, test_multi_lang_splits, test_preserves_filename, test_returns_enqueued (+8) |
| `tests/test_api.py` | make_audio_tensor, _mock_model, test_sync_ratio_calculation, test_sync_ratio_fast, test_sync_ratio_slow (+8) |
| `tests/test_segmentation.py` | _chunks, test_no_mid_word_splits_on_fragmented_whisper, test_no_word_duplicated_across_boundary, test_respects_sentence_boundaries, test_enforces_max_dur (+7) |
| `tests/test_effects_chain.py` | _make_test_audio, test_raw_preset_returns_unmodified, test_broadcast_preset_returns_tensor, test_cinematic_preset_returns_tensor, test_podcast_preset_returns_tensor (+5) |
| `tests/test_dub_transcribe.py` | _make_wav, _seed_job, test_clean_input_preserves_sentence_structure, test_source_lang_detected_and_persisted, _load_fixture (+5) |
| `tests/test_job_store.py` | _unique_id, test_create_mark_done_round_trip, test_mark_failed_carries_error, test_append_event_assigns_monotonic_seq, test_events_since_filters (+3) |
| `backend/tests/test_tts_backend_lifecycle.py` | _load_tts_backend_module, test_unload_defined_on_base_class, test_unload_is_not_abstract, test_unload_signature_takes_self_only, _make_minimal_subclass (+3) |
| `backend/tests/test_atomic_wav.py` | test_writes_valid_wav, test_no_temp_leaks_on_success, test_overwrites_existing_target, test_target_unchanged_when_save_raises, test_no_temp_leaks_on_failure (+2) |
| `tests/test_dub_export_bitrate.py` | _clamp, test_clamp_normal_values_pass_through, test_clamp_below_floor_snaps_to_64k, test_clamp_above_ceiling_snaps_to_320k, test_clamp_malformed_falls_back_to_192k (+2) |
| `backend/tests/test_capture_ws.py` | test_empty_returns_none, test_tiny_returns_none, test_below_100_bytes_returns_none, _src, test_ws_transcribe_references_loopback_hosts (+2) |

## Entry Points

Start here when exploring this area:

- **`test_atomic_save_wav_assembly_pattern`** (Function) — `tests/backend/test_dub_pipeline_wav.py:208`
- **`atomic_save_wav`** (Function) — `backend/services/audio_io.py:264`
- **`test_atomic_save_wav_delegates_to_safe_helper`** (Function) — `tests/backend/services/test_audio_io.py:339`
- **`test_create_mark_done_round_trip`** (Function) — `tests/test_job_store.py:24`
- **`test_mark_failed_carries_error`** (Function) — `tests/test_job_store.py:43`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `test_atomic_save_wav_assembly_pattern` | Function | `tests/backend/test_dub_pipeline_wav.py` | 208 |
| `atomic_save_wav` | Function | `backend/services/audio_io.py` | 264 |
| `test_atomic_save_wav_delegates_to_safe_helper` | Function | `tests/backend/services/test_audio_io.py` | 339 |
| `test_create_mark_done_round_trip` | Function | `tests/test_job_store.py` | 24 |
| `test_mark_failed_carries_error` | Function | `tests/test_job_store.py` | 43 |
| `test_append_event_assigns_monotonic_seq` | Function | `tests/test_job_store.py` | 55 |
| `test_events_since_filters` | Function | `tests/test_job_store.py` | 64 |
| `test_events_respect_per_job_cap` | Function | `tests/test_job_store.py` | 78 |
| `test_list_active_returns_only_live_statuses` | Function | `tests/test_job_store.py` | 99 |
| `test_sweep_orphans_flips_running_to_failed` | Function | `tests/test_job_store.py` | 114 |
| `test_indextts_is_available_returns_tuple` | Function | `tests/test_issue_fixes.py` | 107 |
| `test_indextts_unavailable_message_is_actionable` | Function | `tests/test_issue_fixes.py` | 115 |
| `test_indextts_no_inprocess_import_attempted` | Function | `tests/test_issue_fixes.py` | 136 |
| `test_is_available_no_spawn` | Function | `tests/backend/services/test_indextts_sidecar.py` | 114 |
| `test_is_available_no_venv` | Function | `tests/backend/services/test_indextts_sidecar.py` | 137 |
| `is_indextts_installed` | Function | `backend/engines/indextts/bootstrap.py` | 79 |
| `test_clamp_normal_values_pass_through` | Function | `tests/test_dub_export_bitrate.py` | 30 |
| `test_clamp_below_floor_snaps_to_64k` | Function | `tests/test_dub_export_bitrate.py` | 35 |
| `test_clamp_above_ceiling_snaps_to_320k` | Function | `tests/test_dub_export_bitrate.py` | 40 |
| `test_clamp_malformed_falls_back_to_192k` | Function | `tests/test_dub_export_bitrate.py` | 45 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Enqueue_batch_job → _safe_torchaudio_save` | cross_community | 6 |
| `Ws_transcribe → Find_ffmpeg` | cross_community | 5 |
| `Lifespan → _init_queue` | cross_community | 3 |
| `Lifespan → _push_event` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Routers | 4 calls |
| Cluster_180 | 3 calls |
| Services | 1 calls |
| Indextts | 1 calls |

## How to Explore

1. `gitnexus_context({name: "test_atomic_save_wav_assembly_pattern"})` — see callers and callees
2. `gitnexus_query({query: "tests"})` — find related execution flows
3. Read key files listed above for implementation details
