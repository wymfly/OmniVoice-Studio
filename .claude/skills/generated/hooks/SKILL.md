---
name: hooks
description: "Skill for the Hooks area of OmniVoice-Studio. 128 symbols across 24 files."
---

# Hooks

128 symbols | 24 files | Cohesion: 73%

## When to Use

- Working with code in `frontend/`
- Understanding how setDubJobId, setDubStep, setDubSegments work
- Modifying hooks-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `frontend/src/hooks/useAppData.js` | loadProfiles, loadProjects, projects, profiles, loadAll (+30) |
| `frontend/src/hooks/useDubWorkflow.js` | setDubJobId, setDubStep, setDubSegments, setDubFilename, setDubDuration (+18) |
| `frontend/src/hooks/useSegmentEditing.js` | setDubSegments, pushUndo, undo, redo, editSegments (+10) |
| `frontend/src/App.jsx` | handler, saveProject, App, setShowCheatsheet, h (+4) |
| `frontend/src/hooks/useTTS.js` | useTTS, ingestRefAudio, setText, insertTag, applyPreset (+2) |
| `frontend/src/hooks/useProfiles.js` | useProfiles, setRefText, setInstruct, setLanguage, handleSelectProfile (+2) |
| `frontend/src/store/pillSlice.ts` | showPill, completePill, errorPill, setPillProgress, setPillLabel |
| `frontend/src/api/dub.ts` | transcribeStreamUrl, tasksStreamUrl, listDubHistory, dubTranslate |
| `frontend/src/hooks/useRecording.js` | useRecording, startRecording |
| `frontend/src/utils/media.js` | playBlobAudio, playPing |

## Entry Points

Start here when exploring this area:

- **`setDubJobId`** (Function) — `frontend/src/hooks/useDubWorkflow.js:21`
- **`setDubStep`** (Function) — `frontend/src/hooks/useDubWorkflow.js:23`
- **`setDubSegments`** (Function) — `frontend/src/hooks/useDubWorkflow.js:25`
- **`setDubFilename`** (Function) — `frontend/src/hooks/useDubWorkflow.js:29`
- **`setDubDuration`** (Function) — `frontend/src/hooks/useDubWorkflow.js:30`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `setDubJobId` | Function | `frontend/src/hooks/useDubWorkflow.js` | 21 |
| `setDubStep` | Function | `frontend/src/hooks/useDubWorkflow.js` | 23 |
| `setDubSegments` | Function | `frontend/src/hooks/useDubWorkflow.js` | 25 |
| `setDubFilename` | Function | `frontend/src/hooks/useDubWorkflow.js` | 29 |
| `setDubDuration` | Function | `frontend/src/hooks/useDubWorkflow.js` | 30 |
| `setDubError` | Function | `frontend/src/hooks/useDubWorkflow.js` | 31 |
| `setDubTracks` | Function | `frontend/src/hooks/useDubWorkflow.js` | 32 |
| `setDubTranscript` | Function | `frontend/src/hooks/useDubWorkflow.js` | 33 |
| `setDubProgress` | Function | `frontend/src/hooks/useDubWorkflow.js` | 34 |
| `setDubTaskId` | Function | `frontend/src/hooks/useDubWorkflow.js` | 37 |
| `setDubPrepStage` | Function | `frontend/src/hooks/useDubWorkflow.js` | 38 |
| `setSpeakerClones` | Function | `frontend/src/hooks/useDubWorkflow.js` | 39 |
| `setPreviewSegIds` | Function | `frontend/src/hooks/useDubWorkflow.js` | 40 |
| `_waitForTranscribe` | Function | `frontend/src/hooks/useDubWorkflow.js` | 64 |
| `_waitForPrep` | Function | `frontend/src/hooks/useDubWorkflow.js` | 117 |
| `handleDubUpload` | Function | `frontend/src/hooks/useDubWorkflow.js` | 158 |
| `handleDubIngestUrl` | Function | `frontend/src/hooks/useDubWorkflow.js` | 188 |
| `handleDubRetryTranscribe` | Function | `frontend/src/hooks/useDubWorkflow.js` | 225 |
| `handleDubImportSrt` | Function | `frontend/src/hooks/useDubWorkflow.js` | 241 |
| `handleDubGenerate` | Function | `frontend/src/hooks/useDubWorkflow.js` | 322 |

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
| Api | 24 calls |
| Pages | 8 calls |
| Components | 2 calls |
| Cluster_280 | 1 calls |
| Settings | 1 calls |

## How to Explore

1. `gitnexus_context({name: "setDubJobId"})` — see callers and callees
2. `gitnexus_query({query: "hooks"})` — find related execution flows
3. Read key files listed above for implementation details
