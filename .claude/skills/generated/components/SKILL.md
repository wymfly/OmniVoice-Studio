---
name: components
description: "Skill for the Components area of OmniVoice-Studio. 188 symbols across 34 files."
---

# Components

188 symbols | 34 files | Cohesion: 82%

## When to Use

- Working with code in `frontend/`
- Understanding how GlossaryPanel, pushChange, reload work
- Modifying components-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `frontend/src/components/AudioTrimmer.jsx` | computePeaks, fmtSec, AudioTrimmer, commitStartInput, commitEndInput (+24) |
| `frontend/src/utils/audioTrim.js` | computePeaksFromChannel, computePeaksAsync, probeDuration, cleanup, decodeToMonoLowRate (+10) |
| `frontend/src/components/StoriesEditor.jsx` | fetchChunkAudio, previewTrack, finish, step, StoriesEditor (+10) |
| `frontend/src/components/SearchableSelect.jsx` | readRecents, writeRecents, normalize, SearchableSelect, getVal (+6) |
| `frontend/src/components/GlossaryPanel.jsx` | GlossaryPanel, pushChange, reload, onAdd, onUpdate (+5) |
| `frontend/src/components/CaptureWidget.jsx` | setTrayRecording, formatElapsed, CaptureWidget, handler, applyResult (+4) |
| `frontend/src/components/BootstrapSplash.jsx` | detectHints, formatBytes, BootstrapSplash, handleRetry, handleCleanRetry (+4) |
| `frontend/src/components/ExportModal.jsx` | runSubs, runVideo, runAudio, runStems, runClips (+4) |
| `frontend/src/components/LogsFooter.jsx` | classifyLine, countLevels, LogsFooter, pullFrontend, refreshAll (+3) |
| `frontend/src/components/Sidebar.jsx` | timeAgo, Sidebar, matchesSearch, filteredProjects, filteredProfiles (+3) |

## Entry Points

Start here when exploring this area:

- **`GlossaryPanel`** (Function) — `frontend/src/components/GlossaryPanel.jsx:21`
- **`pushChange`** (Function) — `frontend/src/components/GlossaryPanel.jsx:33`
- **`reload`** (Function) — `frontend/src/components/GlossaryPanel.jsx:35`
- **`onAdd`** (Function) — `frontend/src/components/GlossaryPanel.jsx:51`
- **`onUpdate`** (Function) — `frontend/src/components/GlossaryPanel.jsx:62`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `GlossaryPanel` | Function | `frontend/src/components/GlossaryPanel.jsx` | 21 |
| `pushChange` | Function | `frontend/src/components/GlossaryPanel.jsx` | 33 |
| `reload` | Function | `frontend/src/components/GlossaryPanel.jsx` | 35 |
| `onAdd` | Function | `frontend/src/components/GlossaryPanel.jsx` | 51 |
| `onUpdate` | Function | `frontend/src/components/GlossaryPanel.jsx` | 62 |
| `onDelete` | Function | `frontend/src/components/GlossaryPanel.jsx` | 70 |
| `onClearAuto` | Function | `frontend/src/components/GlossaryPanel.jsx` | 78 |
| `onAutoExtract` | Function | `frontend/src/components/GlossaryPanel.jsx` | 86 |
| `listGlossary` | Function | `frontend/src/api/glossary.ts` | 3 |
| `addGlossaryTerm` | Function | `frontend/src/api/glossary.ts` | 7 |
| `updateGlossaryTerm` | Function | `frontend/src/api/glossary.ts` | 11 |
| `deleteGlossaryTerm` | Function | `frontend/src/api/glossary.ts` | 24 |
| `clearGlossary` | Function | `frontend/src/api/glossary.ts` | 31 |
| `autoExtractGlossary` | Function | `frontend/src/api/glossary.ts` | 46 |
| `computePeaksFromChannel` | Function | `frontend/src/utils/audioTrim.js` | 30 |
| `computePeaksAsync` | Function | `frontend/src/utils/audioTrim.js` | 129 |
| `probeDuration` | Function | `frontend/src/utils/audioTrim.js` | 157 |
| `cleanup` | Function | `frontend/src/utils/audioTrim.js` | 162 |
| `decodeToMonoLowRate` | Function | `frontend/src/utils/audioTrim.js` | 169 |
| `AudioTrimmer` | Function | `frontend/src/components/AudioTrimmer.jsx` | 30 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Sidebar → ApiUrl` | cross_community | 7 |
| `Sidebar → ReadError` | cross_community | 7 |
| `Sidebar → ApiError` | cross_community | 7 |
| `CaptureWidget → GetItem` | cross_community | 7 |
| `CaptureWidget → SetItem` | cross_community | 7 |
| `OnCanvasDown → Clamp` | cross_community | 6 |
| `GlossaryPanel → ApiUrl` | cross_community | 6 |
| `GlossaryPanel → ReadError` | cross_community | 6 |
| `OnClearAuto → ApiUrl` | cross_community | 6 |
| `OnClearAuto → ReadError` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Api | 13 calls |
| Hooks | 12 calls |
| Pages | 10 calls |
| Cluster_280 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "GlossaryPanel"})` — see callers and callees
2. `gitnexus_query({query: "components"})` — find related execution flows
3. Read key files listed above for implementation details
