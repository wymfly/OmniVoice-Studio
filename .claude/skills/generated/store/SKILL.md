---
name: store
description: "Skill for the Store area of OmniVoice-Studio. 21 symbols across 1 files."
---

# Store

21 symbols | 1 files | Cohesion: 100%

## When to Use

- Working with code in `frontend/`
- Understanding how setDubJobId, setDubStep, setDubTaskId work
- Modifying store-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `frontend/src/store/dubSlice.ts` | resolve, setDubJobId, setDubStep, setDubTaskId, setDubPrepStage (+16) |

## Entry Points

Start here when exploring this area:

- **`setDubJobId`** (Function) — `frontend/src/store/dubSlice.ts:154`
- **`setDubStep`** (Function) — `frontend/src/store/dubSlice.ts:155`
- **`setDubTaskId`** (Function) — `frontend/src/store/dubSlice.ts:156`
- **`setDubPrepStage`** (Function) — `frontend/src/store/dubSlice.ts:157`
- **`setDubProgress`** (Function) — `frontend/src/store/dubSlice.ts:158`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `setDubJobId` | Function | `frontend/src/store/dubSlice.ts` | 154 |
| `setDubStep` | Function | `frontend/src/store/dubSlice.ts` | 155 |
| `setDubTaskId` | Function | `frontend/src/store/dubSlice.ts` | 156 |
| `setDubPrepStage` | Function | `frontend/src/store/dubSlice.ts` | 157 |
| `setDubProgress` | Function | `frontend/src/store/dubSlice.ts` | 158 |
| `setDubError` | Function | `frontend/src/store/dubSlice.ts` | 159 |
| `setIsTranslating` | Function | `frontend/src/store/dubSlice.ts` | 160 |
| `setDubSegments` | Function | `frontend/src/store/dubSlice.ts` | 161 |
| `setDubTranscript` | Function | `frontend/src/store/dubSlice.ts` | 162 |
| `setDubFilename` | Function | `frontend/src/store/dubSlice.ts` | 163 |
| `setDubDuration` | Function | `frontend/src/store/dubSlice.ts` | 164 |
| `setDubTracks` | Function | `frontend/src/store/dubSlice.ts` | 165 |
| `setDubLang` | Function | `frontend/src/store/dubSlice.ts` | 166 |
| `setDubLangCode` | Function | `frontend/src/store/dubSlice.ts` | 167 |
| `setDubInstruct` | Function | `frontend/src/store/dubSlice.ts` | 168 |
| `setPreserveBg` | Function | `frontend/src/store/dubSlice.ts` | 169 |
| `setDefaultTrack` | Function | `frontend/src/store/dubSlice.ts` | 170 |
| `setExportTracks` | Function | `frontend/src/store/dubSlice.ts` | 171 |
| `setPreviewSegIds` | Function | `frontend/src/store/dubSlice.ts` | 172 |
| `setSpeakerClones` | Function | `frontend/src/store/dubSlice.ts` | 173 |

## How to Explore

1. `gitnexus_context({name: "setDubJobId"})` — see callers and callees
2. `gitnexus_query({query: "store"})` — find related execution flows
3. Read key files listed above for implementation details
