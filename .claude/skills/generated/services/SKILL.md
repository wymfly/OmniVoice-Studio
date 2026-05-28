---
name: services
description: "Skill for the Services area of OmniVoice-Studio. 352 symbols across 54 files."
---

# Services

352 symbols | 54 files | Cohesion: 86%

## When to Use

- Working with code in `backend/`
- Understanding how test_smoke_3langs_3sec, echo_backend, test_env_forwarding_contract work
- Modifying services-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `backend/services/tts_backend.py` | TTSBackend, OmniVoiceBackend, VoxCPM2Backend, MossTTSNanoBackend, KittenTTSBackend (+27) |
| `backend/services/asr_backend.py` | unload, is_available, _ensure_pipe, transcribe, ASRBackend (+26) |
| `backend/services/model_manager.py` | _classify_diarization_error, get_diarization_pipeline, get_model, _lazy_omnivoice, _set_loading (+15) |
| `tests/backend/services/test_audio_io.py` | test_safe_save_out_of_range_clamped, test_safe_save_non_contiguous_via_transpose, test_safe_save_rejects_empty_tensor, test_safe_save_rejects_non_tensor, test_safe_save_handles_1d_tensor (+13) |
| `backend/services/segmentation.py` | assign_speakers_from_diarization, assign_speakers_heuristic, _word_count, _is_short, _is_ultra_short (+11) |
| `backend/services/subprocess_backend.py` | venv_python, sidecar_script, _spawn, shutdown, _force_kill (+9) |
| `backend/services/dub_pipeline.py` | safe_job_dir, prep_event, find_cached_job, kill_job_procs, put_job (+8) |
| `backend/services/watermark.py` | is_visible_audio_enabled, is_visible_video_enabled, generate_brand_tone, apply_audio_brand, get_ffmpeg_overlay_args (+6) |
| `backend/services/subtitle_segmenter.py` | segment_for_subtitles, _to_seg, _from_seg, _merge_tiny_neighbours, _should_merge (+6) |
| `tests/backend/services/test_indextts_sidecar.py` | patched_indextts_backend, test_env_forwarding_to_indextts_sidecar, test_synthesize_via_mocked_sidecar, test_synthesize_forwards_emotion_kwargs_via_vector, test_synthesize_forwards_emotion_kwargs_via_text (+5) |

## Entry Points

Start here when exploring this area:

- **`test_smoke_3langs_3sec`** (Function) — `tests/test_supertonic3.py:253`
- **`echo_backend`** (Function) — `tests/backend/services/test_subprocess_backend.py:73`
- **`test_env_forwarding_contract`** (Function) — `tests/backend/services/test_subprocess_backend.py:155`
- **`test_oversize_frame_rejected`** (Function) — `tests/backend/services/test_subprocess_backend.py:226`
- **`test_short_read_rejected`** (Function) — `tests/backend/services/test_subprocess_backend.py:244`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `TTSBackend` | Class | `backend/services/tts_backend.py` | 58 |
| `OmniVoiceBackend` | Class | `backend/services/tts_backend.py` | 154 |
| `VoxCPM2Backend` | Class | `backend/services/tts_backend.py` | 231 |
| `MossTTSNanoBackend` | Class | `backend/services/tts_backend.py` | 342 |
| `KittenTTSBackend` | Class | `backend/services/tts_backend.py` | 432 |
| `MLXAudioBackend` | Class | `backend/services/tts_backend.py` | 526 |
| `CosyVoiceBackend` | Class | `backend/services/tts_backend.py` | 648 |
| `GPTSoVITSBackend` | Class | `backend/services/tts_backend.py` | 812 |
| `SherpaOnnxBackend` | Class | `backend/services/tts_backend.py` | 922 |
| `BrokenBackend` | Class | `tests/backend/services/test_tts_backend_registry.py` | 50 |
| `HealthyInProcessBackend` | Class | `tests/backend/services/test_tts_backend_registry.py` | 70 |
| `FlakyBackend` | Class | `tests/backend/services/test_tts_backend_registry.py` | 176 |
| `ASRBackend` | Class | `backend/services/asr_backend.py` | 36 |
| `WhisperXBackend` | Class | `backend/services/asr_backend.py` | 60 |
| `FasterWhisperBackend` | Class | `backend/services/asr_backend.py` | 260 |
| `MLXWhisperBackend` | Class | `backend/services/asr_backend.py` | 375 |
| `PyTorchWhisperBackend` | Class | `backend/services/asr_backend.py` | 439 |
| `NeMoASRBackend` | Class | `backend/services/asr_backend.py` | 495 |
| `MoonshineASRBackend` | Class | `backend/services/asr_backend.py` | 604 |
| `SubprocessBackend` | Class | `backend/services/subprocess_backend.py` | 94 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Dub_translate → Is_available` | cross_community | 9 |
| `Enqueue_batch_job → _lazy_torch` | cross_community | 9 |
| `Dub_translate → Is_empty` | cross_community | 7 |
| `Dub_translate → Instruct_prompt` | cross_community | 7 |
| `Dub_translate → Chat` | cross_community | 7 |
| `Dub_translate → _heuristic_parse` | cross_community | 7 |
| `Dub_translate → _normalize` | cross_community | 7 |
| `Setup_warmup → _lazy_torch` | cross_community | 7 |
| `Export_file → _load` | cross_community | 6 |
| `Ws_tts → _lazy_torch` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Routers | 24 calls |
| Tests | 1 calls |

## How to Explore

1. `gitnexus_context({name: "test_smoke_3langs_3sec"})` — see callers and callees
2. `gitnexus_query({query: "services"})` — find related execution flows
3. Read key files listed above for implementation details
