---
name: settings
description: "Skill for the Settings area of OmniVoice-Studio. 10 symbols across 3 files."
---

# Settings

10 symbols | 3 files | Cohesion: 79%

## When to Use

- Working with code in `frontend/`
- Understanding how PerformancePanel, setShowHeaderLiveStats, refresh work
- Modifying settings-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `frontend/src/components/settings/PerformancePanel.jsx` | PerformancePanel, setShowHeaderLiveStats, refresh, onToggle |
| `frontend/src/components/settings/ApiKeysPanel.jsx` | ApiKeysPanel, refresh, onSave, onClear |
| `frontend/src/components/settings/AppearancePanel.jsx` | AppearancePanel, setTheme |

## Entry Points

Start here when exploring this area:

- **`PerformancePanel`** (Function) — `frontend/src/components/settings/PerformancePanel.jsx:23`
- **`setShowHeaderLiveStats`** (Function) — `frontend/src/components/settings/PerformancePanel.jsx:33`
- **`refresh`** (Function) — `frontend/src/components/settings/PerformancePanel.jsx:35`
- **`onToggle`** (Function) — `frontend/src/components/settings/PerformancePanel.jsx:58`
- **`ApiKeysPanel`** (Function) — `frontend/src/components/settings/ApiKeysPanel.jsx:47`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `PerformancePanel` | Function | `frontend/src/components/settings/PerformancePanel.jsx` | 23 |
| `setShowHeaderLiveStats` | Function | `frontend/src/components/settings/PerformancePanel.jsx` | 33 |
| `refresh` | Function | `frontend/src/components/settings/PerformancePanel.jsx` | 35 |
| `onToggle` | Function | `frontend/src/components/settings/PerformancePanel.jsx` | 58 |
| `ApiKeysPanel` | Function | `frontend/src/components/settings/ApiKeysPanel.jsx` | 47 |
| `refresh` | Function | `frontend/src/components/settings/ApiKeysPanel.jsx` | 56 |
| `onSave` | Function | `frontend/src/components/settings/ApiKeysPanel.jsx` | 73 |
| `onClear` | Function | `frontend/src/components/settings/ApiKeysPanel.jsx` | 89 |
| `AppearancePanel` | Function | `frontend/src/components/settings/AppearancePanel.jsx` | 23 |
| `setTheme` | Function | `frontend/src/components/settings/AppearancePanel.jsx` | 27 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `OnToggle → ApiUrl` | cross_community | 5 |
| `OnToggle → ReadError` | cross_community | 5 |
| `OnToggle → ApiError` | cross_community | 5 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Api | 4 calls |

## How to Explore

1. `gitnexus_context({name: "PerformancePanel"})` — see callers and callees
2. `gitnexus_query({query: "settings"})` — find related execution flows
3. Read key files listed above for implementation details
