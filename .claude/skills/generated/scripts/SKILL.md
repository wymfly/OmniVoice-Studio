---
name: scripts
description: "Skill for the Scripts area of OmniVoice-Studio. 105 symbols across 16 files."
---

# Scripts

105 symbols | 16 files | Cohesion: 93%

## When to Use

- Working with code in `omnivoice/`
- Understanding how test_clean_state_passes, test_drift_introduced_fails, test_skip_marker_allows_divergence work
- Modifying scripts-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `omnivoice/scripts/denoise_audio.py` | size, extract_seamless_m4t_features, _pad_batch, process, process_batch (+15) |
| `omnivoice/scripts/extract_audio_tokens_add_noise.py` | build_parser, count_lines, main, open_new_shard, handle_result (+12) |
| `tests/scripts/test_validate_install_docs.py` | _make_root, test_clean_state_passes, test_drift_introduced_fails, test_skip_marker_allows_divergence, test_skip_marker_diverging_block_exit_zero (+6) |
| `omnivoice/scripts/extract_audio_tokens.py` | build_parser, count_lines, main, open_new_shard, handle_result (+5) |
| `scripts/resolve_supertonic3_sha.py` | _read_current_sha, _commit_touches_inference, _iter_main_commits, resolve, _sha (+2) |
| `scripts/bench_incremental.py` | post, stream_sse, wait_prep, transcribe, to_dub_segment (+2) |
| `scripts/seed-test-fixture.py` | write_silence_wav, write_profile_json, build_database, write_readme, directory_size_bytes (+1) |
| `scripts/validate-install-docs.py` | _normalise_line, _normalise_script, _extract_validated_blocks, _iter_docs, main |
| `scripts/setup.py` | _ensure_vcredist_windows, _find_compat_dir, _cudnn8_lib_dir, _count_cudnn8_libs, main |
| `omnivoice/scripts/jsonl_to_webdataset.py` | read_jsonl, chunked_reader, count_lines, pack_dataset, submit_next_chunks |

## Entry Points

Start here when exploring this area:

- **`test_clean_state_passes`** (Function) — `tests/scripts/test_validate_install_docs.py:54`
- **`test_drift_introduced_fails`** (Function) — `tests/scripts/test_validate_install_docs.py:74`
- **`test_skip_marker_allows_divergence`** (Function) — `tests/scripts/test_validate_install_docs.py:95`
- **`test_skip_marker_diverging_block_exit_zero`** (Function) — `tests/scripts/test_validate_install_docs.py:114`
- **`test_prompt_prefix_stripped`** (Function) — `tests/scripts/test_validate_install_docs.py:132`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `test_clean_state_passes` | Function | `tests/scripts/test_validate_install_docs.py` | 54 |
| `test_drift_introduced_fails` | Function | `tests/scripts/test_validate_install_docs.py` | 74 |
| `test_skip_marker_allows_divergence` | Function | `tests/scripts/test_validate_install_docs.py` | 95 |
| `test_skip_marker_diverging_block_exit_zero` | Function | `tests/scripts/test_validate_install_docs.py` | 114 |
| `test_prompt_prefix_stripped` | Function | `tests/scripts/test_validate_install_docs.py` | 132 |
| `test_python_prompt_prefix_stripped` | Function | `tests/scripts/test_validate_install_docs.py` | 149 |
| `test_crlf_normalization` | Function | `tests/scripts/test_validate_install_docs.py` | 166 |
| `test_trailing_whitespace_tolerated` | Function | `tests/scripts/test_validate_install_docs.py` | 185 |
| `test_blank_and_comment_only_lines_skipped` | Function | `tests/scripts/test_validate_install_docs.py` | 202 |
| `test_true_diff_distinguished_from_whitespace` | Function | `tests/scripts/test_validate_install_docs.py` | 223 |
| `id` | Function | `frontend/src/pages/DubTab.jsx` | 114 |
| `label` | Function | `frontend/src/components/FloatingPill.jsx` | 39 |
| `run` | Function | `frontend/src-tauri/src/lib.rs` | 60 |
| `default_dictation_shortcut` | Function | `frontend/src-tauri/src/config.rs` | 38 |
| `load_config_pre_app` | Function | `frontend/src-tauri/src/config.rs` | 67 |
| `simulate_paste` | Function | `frontend/src-tauri/src/commands.rs` | 260 |
| `resolve` | Function | `scripts/resolve_supertonic3_sha.py` | 103 |
| `main` | Function | `scripts/resolve_supertonic3_sha.py` | 178 |
| `post` | Function | `scripts/bench_incremental.py` | 31 |
| `stream_sse` | Function | `scripts/bench_incremental.py` | 42 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Main → _pad_batch` | cross_community | 5 |
| `Run → Config_path_pre_app` | intra_community | 3 |
| `Main → _subprocess_recv` | cross_community | 3 |
| `Main → _subprocess_send` | cross_community | 3 |
| `Main → _normalise_line` | intra_community | 3 |
| `Main → Stream_sse` | intra_community | 3 |
| `Main → To_dub_segment` | intra_community | 3 |
| `Main → Post` | intra_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Pages | 4 calls |
| Test | 4 calls |
| Cluster_362 | 2 calls |

## How to Explore

1. `gitnexus_context({name: "test_clean_state_passes"})` — see callers and callees
2. `gitnexus_query({query: "scripts"})` — find related execution flows
3. Read key files listed above for implementation details
