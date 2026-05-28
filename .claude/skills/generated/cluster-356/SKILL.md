---
name: cluster-356
description: "Skill for the Cluster_356 area of OmniVoice-Studio. 12 symbols across 2 files."
---

# Cluster_356

12 symbols | 2 files | Cohesion: 72%

## When to Use

- Working with code in `frontend/`
- Understanding how find_bundled_sidecar, find_bundled_uv, find_bundled_ffmpeg work
- Modifying cluster_356-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `frontend/src-tauri/src/tools.rs` | find_bundled_sidecar, find_bundled_uv, find_bundled_ffmpeg, find_bundled_ffprobe, install_ffmpeg_standalone (+4) |
| `frontend/src-tauri/src/config.rs` | resolve_github_url, auto_detect_region, get_effective_region |

## Entry Points

Start here when exploring this area:

- **`find_bundled_sidecar`** (Function) — `frontend/src-tauri/src/tools.rs:43`
- **`find_bundled_uv`** (Function) — `frontend/src-tauri/src/tools.rs:69`
- **`find_bundled_ffmpeg`** (Function) — `frontend/src-tauri/src/tools.rs:70`
- **`find_bundled_ffprobe`** (Function) — `frontend/src-tauri/src/tools.rs:71`
- **`install_ffmpeg_standalone`** (Function) — `frontend/src-tauri/src/tools.rs:83`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `find_bundled_sidecar` | Function | `frontend/src-tauri/src/tools.rs` | 43 |
| `find_bundled_uv` | Function | `frontend/src-tauri/src/tools.rs` | 69 |
| `find_bundled_ffmpeg` | Function | `frontend/src-tauri/src/tools.rs` | 70 |
| `find_bundled_ffprobe` | Function | `frontend/src-tauri/src/tools.rs` | 71 |
| `install_ffmpeg_standalone` | Function | `frontend/src-tauri/src/tools.rs` | 83 |
| `resolve_ffmpeg` | Function | `frontend/src-tauri/src/tools.rs` | 277 |
| `resolve_ffprobe` | Function | `frontend/src-tauri/src/tools.rs` | 324 |
| `resolve_uv` | Function | `frontend/src-tauri/src/tools.rs` | 372 |
| `resolve_github_url` | Function | `frontend/src-tauri/src/config.rs` | 96 |
| `auto_detect_region` | Function | `frontend/src-tauri/src/config.rs` | 105 |
| `get_effective_region` | Function | `frontend/src-tauri/src/config.rs` | 123 |
| `install_uv_standalone` | Function | `frontend/src-tauri/src/tools.rs` | 400 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Services | 5 calls |
| Pages | 1 calls |
| Cluster_359 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "find_bundled_sidecar"})` — see callers and callees
2. `gitnexus_query({query: "cluster_356"})` — find related execution flows
3. Read key files listed above for implementation details
