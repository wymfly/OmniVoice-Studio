---
name: pages
description: "Skill for the Pages area of OmniVoice-Studio. 110 symbols across 24 files."
---

# Pages

110 symbols | 24 files | Cohesion: 73%

## When to Use

- Working with code in `frontend/`
- Understanding how DubTab, setDubStep, setDubSegments work
- Modifying pages-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `frontend/src/pages/Settings.jsx` | lines, isTauri, Settings, copyDiagnostics, fmtGB (+14) |
| `frontend/src/pages/DubTab.jsx` | DubTab, setDubStep, setDubSegments, setDubLang, setDubLangCode (+11) |
| `frontend/src/pages/VoiceGallery.jsx` | VoiceGallery, loadVoices, handleDownload, handleSaveAsProfile, handleDeleteVoice (+3) |
| `frontend/src/api/hooks.ts` | galleryVoices, useGalleryCategories, useGalleryVoices, useSysinfo, useSystemInfo (+3) |
| `frontend/src/pages/Transcriptions.jsx` | loadTranscriptions, handler, saveTranscriptions, clearAll, TranscriptionsPage (+3) |
| `frontend/src-tauri/src/bootstrap.rs` | set_stage, emit_log, run_streaming, venv_python_path, copy_dir_recursive (+2) |
| `frontend/src/pages/BatchQueue.jsx` | BatchQueue, reload, handleEnqueue, handleCancel, JobCard (+2) |
| `frontend/src/pages/Projects.jsx` | fmtTime, Projects, handler, fmtDuration, items |
| `frontend/src/pages/VoiceProfile.jsx` | VoiceProfile, reload, onUnlock, onDelete |
| `frontend/src/api/profiles.ts` | getProfile, getProfileUsage, unlockProfile, deleteProfile |

## Entry Points

Start here when exploring this area:

- **`DubTab`** (Function) — `frontend/src/pages/DubTab.jsx:31`
- **`setDubStep`** (Function) — `frontend/src/pages/DubTab.jsx:58`
- **`setDubSegments`** (Function) — `frontend/src/pages/DubTab.jsx:63`
- **`setDubLang`** (Function) — `frontend/src/pages/DubTab.jsx:66`
- **`setDubLangCode`** (Function) — `frontend/src/pages/DubTab.jsx:68`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `DubTab` | Function | `frontend/src/pages/DubTab.jsx` | 31 |
| `setDubStep` | Function | `frontend/src/pages/DubTab.jsx` | 58 |
| `setDubSegments` | Function | `frontend/src/pages/DubTab.jsx` | 63 |
| `setDubLang` | Function | `frontend/src/pages/DubTab.jsx` | 66 |
| `setDubLangCode` | Function | `frontend/src/pages/DubTab.jsx` | 68 |
| `setDubInstruct` | Function | `frontend/src/pages/DubTab.jsx` | 70 |
| `setPreserveBg` | Function | `frontend/src/pages/DubTab.jsx` | 76 |
| `setDefaultTrack` | Function | `frontend/src/pages/DubTab.jsx` | 78 |
| `setExportTracks` | Function | `frontend/src/pages/DubTab.jsx` | 80 |
| `setIsSidebarCollapsed` | Function | `frontend/src/pages/DubTab.jsx` | 83 |
| `setDualSubs` | Function | `frontend/src/pages/DubTab.jsx` | 87 |
| `setBurnSubs` | Function | `frontend/src/pages/DubTab.jsx` | 89 |
| `onIngestUrl` | Function | `frontend/src/pages/DubTab.jsx` | 200 |
| `emit` | Function | `backend/core/event_bus.py` | 43 |
| `lines` | Function | `frontend/src/pages/Settings.jsx` | 964 |
| `set_stage` | Function | `frontend/src-tauri/src/bootstrap.rs` | 43 |
| `emit_log` | Function | `frontend/src-tauri/src/bootstrap.rs` | 57 |
| `run_streaming` | Function | `frontend/src-tauri/src/bootstrap.rs` | 70 |
| `venv_python_path` | Function | `frontend/src-tauri/src/bootstrap.rs` | 217 |
| `copy_dir_recursive` | Function | `frontend/src-tauri/src/bootstrap.rs` | 226 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `DubTab → ApiUrl` | cross_community | 7 |
| `DubTab → ReadError` | cross_community | 7 |
| `DubTab → ApiError` | cross_community | 7 |
| `CaptureWidget → GetItem` | cross_community | 7 |
| `CaptureWidget → SetItem` | cross_community | 7 |
| `CloneDesignTab → ApiUrl` | cross_community | 7 |
| `CloneDesignTab → ReadError` | cross_community | 7 |
| `CloneDesignTab → ApiError` | cross_community | 7 |
| `OnUnlock → ApiUrl` | cross_community | 6 |
| `OnUnlock → ReadError` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Api | 11 calls |
| Hooks | 8 calls |
| Cluster_359 | 4 calls |
| Components | 2 calls |
| Services | 1 calls |
| Cluster_362 | 1 calls |
| Test | 1 calls |

## How to Explore

1. `gitnexus_context({name: "DubTab"})` — see callers and callees
2. `gitnexus_query({query: "pages"})` — find related execution flows
3. Read key files listed above for implementation details
