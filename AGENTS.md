<!-- gitnexus:start -->
# GitNexus — Code Intelligence

This project is indexed by GitNexus as **OmniVoice-Studio** (11411 symbols, 18394 relationships, 300 execution flows). Use the GitNexus MCP tools to understand code, assess impact, and navigate safely.

> If any GitNexus tool warns the index is stale, run `npx gitnexus analyze` in terminal first.

## Always Do

- **MUST run impact analysis before editing any symbol.** Before modifying a function, class, or method, run `gitnexus_impact({target: "symbolName", direction: "upstream"})` and report the blast radius (direct callers, affected processes, risk level) to the user.
- **MUST run `gitnexus_detect_changes()` before committing** to verify your changes only affect expected symbols and execution flows.
- **MUST warn the user** if impact analysis returns HIGH or CRITICAL risk before proceeding with edits.
- When exploring unfamiliar code, use `gitnexus_query({query: "concept"})` to find execution flows instead of grepping. It returns process-grouped results ranked by relevance.
- When you need full context on a specific symbol — callers, callees, which execution flows it participates in — use `gitnexus_context({name: "symbolName"})`.

## Never Do

- NEVER edit a function, class, or method without first running `gitnexus_impact` on it.
- NEVER ignore HIGH or CRITICAL risk warnings from impact analysis.
- NEVER rename symbols with find-and-replace — use `gitnexus_rename` which understands the call graph.
- NEVER commit changes without running `gitnexus_detect_changes()` to check affected scope.

## Resources

| Resource | Use for |
|----------|---------|
| `gitnexus://repo/OmniVoice-Studio/context` | Codebase overview, check index freshness |
| `gitnexus://repo/OmniVoice-Studio/clusters` | All functional areas |
| `gitnexus://repo/OmniVoice-Studio/processes` | All execution flows |
| `gitnexus://repo/OmniVoice-Studio/process/{name}` | Step-by-step execution trace |

## CLI

| Task | Read this skill file |
|------|---------------------|
| Understand architecture / "How does X work?" | `.claude/skills/gitnexus/gitnexus-exploring/SKILL.md` |
| Blast radius / "What breaks if I change X?" | `.claude/skills/gitnexus/gitnexus-impact-analysis/SKILL.md` |
| Trace bugs / "Why is X failing?" | `.claude/skills/gitnexus/gitnexus-debugging/SKILL.md` |
| Rename / extract / split / refactor | `.claude/skills/gitnexus/gitnexus-refactoring/SKILL.md` |
| Tools, resources, schema reference | `.claude/skills/gitnexus/gitnexus-guide/SKILL.md` |
| Index, status, clean, wiki CLI commands | `.claude/skills/gitnexus/gitnexus-cli/SKILL.md` |
| Work in the Services area (352 symbols) | `.claude/skills/generated/services/SKILL.md` |
| Work in the Components area (188 symbols) | `.claude/skills/generated/components/SKILL.md` |
| Work in the Routers area (165 symbols) | `.claude/skills/generated/routers/SKILL.md` |
| Work in the Tests area (141 symbols) | `.claude/skills/generated/tests/SKILL.md` |
| Work in the Api area (129 symbols) | `.claude/skills/generated/api/SKILL.md` |
| Work in the Hooks area (128 symbols) | `.claude/skills/generated/hooks/SKILL.md` |
| Work in the Pages area (110 symbols) | `.claude/skills/generated/pages/SKILL.md` |
| Work in the Scripts area (105 symbols) | `.claude/skills/generated/scripts/SKILL.md` |
| Work in the Wer area (48 symbols) | `.claude/skills/generated/wer/SKILL.md` |
| Work in the Models area (46 symbols) | `.claude/skills/generated/models/SKILL.md` |
| Work in the Backend area (34 symbols) | `.claude/skills/generated/backend/SKILL.md` |
| Work in the Cli area (28 symbols) | `.claude/skills/generated/cli/SKILL.md` |
| Work in the Setup area (27 symbols) | `.claude/skills/generated/setup/SKILL.md` |
| Work in the Omnivoice_gguf area (26 symbols) | `.claude/skills/generated/omnivoice-gguf/SKILL.md` |
| Work in the Store area (21 symbols) | `.claude/skills/generated/store/SKILL.md` |
| Work in the Training area (18 symbols) | `.claude/skills/generated/training/SKILL.md` |
| Work in the Data area (16 symbols) | `.claude/skills/generated/data/SKILL.md` |
| Work in the Cluster_356 area (12 symbols) | `.claude/skills/generated/cluster-356/SKILL.md` |
| Work in the Indextts area (12 symbols) | `.claude/skills/generated/indextts/SKILL.md` |
| Work in the Settings area (10 symbols) | `.claude/skills/generated/settings/SKILL.md` |

<!-- gitnexus:end -->
