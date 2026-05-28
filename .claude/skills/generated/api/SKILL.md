---
name: api
description: "Skill for the Api area of OmniVoice-Studio. 129 symbols across 25 files."
---

# Api

129 symbols | 25 files | Cohesion: 74%

## When to Use

- Working with code in `frontend/`
- Understanding how rustData, modelStatus, systemInfo work
- Modifying api-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `frontend/src/App.jsx` | setMode, setDubJobId, setDubStep, setDubSegments, setDubLang (+17) |
| `tests/backend/api/test_engines_route_shape.py` | _client, test_engines_response_includes_new_fields, test_indextts2_entry_has_subprocess_isolation_mode, test_omnivoice_entry_has_in_process_isolation_mode, test_gpu_compat_omnivoice_has_cuda_mps_cpu (+7) |
| `frontend/src/api/system.ts` | rustData, modelStatus, systemInfo, getInvoke, invokeOrFetch (+6) |
| `frontend/src/api/gallery.ts` | listCategories, getGalleryVoice, searchYoutube, downloadYoutubeClip, saveVoiceAsProfile (+6) |
| `frontend/src/api/engines.ts` | listEngines, listTtsBackends, listAsrBackends, listLlmBackends, getEngineHealth (+6) |
| `frontend/src/api/hooks.ts` | queryFn, useModels, useRecommendations, useInstallModel, useDeleteModel (+6) |
| `frontend/src/api/dub.ts` | dubAbort, tasksCancel, clearDubHistory, dubUpload, dubIngestUrl (+3) |
| `frontend/src/api/setup.ts` | listModels, getRecommendations, preflight, setupWarmup, setupDownloadStreamUrl (+2) |
| `frontend/src/api/client.ts` | apiJson, ApiError, readError, apiFetch, apiPost (+2) |
| `frontend/src/pages/Settings.jsx` | onSelect, refreshLogs, ModelStoreTab, saveHfToken, onClearLogs |

## Entry Points

Start here when exploring this area:

- **`rustData`** (Function) — `frontend/src/api/system.ts:58`
- **`modelStatus`** (Function) — `frontend/src/api/system.ts:88`
- **`systemInfo`** (Function) — `frontend/src/api/system.ts:101`
- **`listModels`** (Function) — `frontend/src/api/setup.ts:56`
- **`getRecommendations`** (Function) — `frontend/src/api/setup.ts:94`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ApiError` | Class | `frontend/src/api/client.ts` | 6 |
| `rustData` | Function | `frontend/src/api/system.ts` | 58 |
| `modelStatus` | Function | `frontend/src/api/system.ts` | 88 |
| `systemInfo` | Function | `frontend/src/api/system.ts` | 101 |
| `listModels` | Function | `frontend/src/api/setup.ts` | 56 |
| `getRecommendations` | Function | `frontend/src/api/setup.ts` | 94 |
| `preflight` | Function | `frontend/src/api/setup.ts` | 139 |
| `listProjects` | Function | `frontend/src/api/projects.ts` | 3 |
| `loadProject` | Function | `frontend/src/api/projects.ts` | 12 |
| `listProfiles` | Function | `frontend/src/api/profiles.ts` | 3 |
| `listCategories` | Function | `frontend/src/api/gallery.ts` | 25 |
| `getGalleryVoice` | Function | `frontend/src/api/gallery.ts` | 32 |
| `searchYoutube` | Function | `frontend/src/api/gallery.ts` | 44 |
| `downloadYoutubeClip` | Function | `frontend/src/api/gallery.ts` | 62 |
| `saveVoiceAsProfile` | Function | `frontend/src/api/gallery.ts` | 70 |
| `listEngines` | Function | `frontend/src/api/engines.ts` | 33 |
| `listTtsBackends` | Function | `frontend/src/api/engines.ts` | 37 |
| `listAsrBackends` | Function | `frontend/src/api/engines.ts` | 40 |
| `listLlmBackends` | Function | `frontend/src/api/engines.ts` | 43 |
| `getEngineHealth` | Function | `frontend/src/api/engines.ts` | 62 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `DubTab → ApiUrl` | cross_community | 7 |
| `DubTab → ReadError` | cross_community | 7 |
| `DubTab → ApiError` | cross_community | 7 |
| `Sidebar → ApiUrl` | cross_community | 7 |
| `Sidebar → ReadError` | cross_community | 7 |
| `Sidebar → ApiError` | cross_community | 7 |
| `OnCheckpointContinue → ApiUrl` | cross_community | 7 |
| `OnCheckpointContinue → ReadError` | cross_community | 7 |
| `OnCheckpointContinue → ApiError` | cross_community | 7 |
| `CloneDesignTab → ApiUrl` | cross_community | 7 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Pages | 7 calls |
| Hooks | 7 calls |
| Components | 1 calls |

## How to Explore

1. `gitnexus_context({name: "rustData"})` — see callers and callees
2. `gitnexus_query({query: "api"})` — find related execution flows
3. Read key files listed above for implementation details
