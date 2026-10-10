# MK231 Git / ZIP push–pull contract — adopted workflow

## Local topology

```
%USERPROFILE%\MK231\           # Local working directory + Git repository root
├── _inbox\                     # LOCAL ONLY, ignored by Git; future cumulative ZIP deliveries
├── Executable.md               # Included in repo as Codex-oriented runbook
├── AGENTS.md                   # Continuity constitution for AI coding assistants
├── README.md                   # Project navigator
├── CURRENT_LIVE_MODEL.md
├── canon\ story\ constitution\ workshop\ visuals\ provenance\ history\ scripts\
└── .git\                      # Created by Git, never shipped in ZIP
```

The screenshot shows a new Windows `MK231` folder containing `_inbox`. Earlier spoken 'MK31' is not adopted as the repository name; the explicit URL and screenshot identify MK231. Avoid embedding the local Windows username or machine-specific drive letter in the repo. Use `%USERPROFILE%` or an explicitly author-selected location. Do not commit photographs of Windows Explorer just to show this workflow.

**Remote:** `https://github.com/xApologies/MK231` (exists and was empty at handoff audit). This ZIP does NOT create a remote commit by itself; Codex does that later.

## Ingestion protocol

1. Download the dated/versioned ZIP into `_inbox` unchanged.
2. Tell Codex to read `Executable.md` from the archive.
3. Codex checks repo state, stages extraction away from root, verifies checksums, compares history and transfers approved content.
4. Codex commits/pushes without touching `_inbox` or overwriting other repository work.
5. Once upload is confirmed, Git's latest `main` is the durable working state. The original archive remains retrievable from local `_inbox`; provenance copies live inside committed project directories.

## Future incremental packages

- Prefer **cumulative**, self-contained packages with all current essential files, archived source and an explicit change log. Newest author decisions supersede inconsistent summaries.
- Avoid ZIP-inside-ZIP proliferation unless intentionally preserving an original checkpoint archive for chain-of-custody; this release intentionally preserves the exact v0.3.0 source ZIP once.
- `Executable.md` must state whether it is full bootstrap or delta, target branch, status of `_inbox`, expected paths, and verification checks.
- Before updating Git, compare to current HEAD, retain `history` and `provenance`, and communicate conflicts. Never use `git push --force`.
- The tools may clone/commit when the author authorizes but no assistant should claim success without the remote commit SHA.

## v1.1 publication contract

Root `CONSTITUTION.md` is mandatory, self-contained and linked from README/AGENTS. Preserve newer root edits and synchronize approved specialized changes. Each semantic release compares every substantive incoming decision against live remote main, records destinations/statuses and unresolved gaps in a reconciliation report, validates assets/links/checksums, and reports the actual remote commit SHA. `_inbox` and staging remain ignored and untracked. Historical source records are immutable.
