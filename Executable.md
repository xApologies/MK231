# Executable.md — MK231 v1.1.0 Semantic Reconciliation Update

**MODE: INCREMENTAL SEMANTIC UPDATE; NOT FULL REPOSITORY REPLACEMENT.**
**Target:** https://github.com/xApologies/MK231
**Branch:** main
**Local working folder:** `%USERPROFILE%\\MK231`
**Local ZIP inbox:** `_inbox/` (must remain untracked)
**Expected earlier Git SHA when audited:** `61c15595454360757e947a7fda0e7b95b8d98d2d`. DO NOT assume it is still HEAD.

## Execution instructions
1. Check local `git status`, branch, remote URL, fetch origin, and inspect the current remote `main`. If dirty or conflicted, STOP and report; don't discard anything.
2. Extract this ZIP into a **temporary staging directory outside Git-tracked files**; verify `SHA256SUMS.txt`. Never stage `_inbox`, ZIPs in `_inbox`, or temporary extraction paths.
3. Read `provenance/REVERSE_DIFF_v1.1.md` and all `updates/*.md`. Compare **every substantive decision** against the current repository, not only filenames. Inspect existing `CURRENT_LIVE_MODEL.md`, `canon/`, `story/`, `constitution/`, `provenance/`, `AGENTS.md`, `README.md`.
4. Merge the updates into appropriate existing canonical documents and `CURRENT_LIVE_MODEL.md`, preserving all existing material. This update does not authorize wholesale replacement of current files or cloning MK147/MK157/_bricked.
5. **Root CONSTITUTION.md is mandatory.** A separate Codex task to restore it may have completed. Compare the current root file against this ZIP's updated cumulative version. Preserve all newer existing changes, merge Part D amendments, and ensure the root file remains self-contained. Do not overwrite another Codex run's work. Keep specialized constitutions. Link root constitution from README and AGENTS.
6. Critical semantic lock: NEW book labels I Red/Phoenix, II Orange/Kitsune, III Yellow/Dragon, IV Green/Unicorn, V Blue/Primordial, VI Violet/Leviathan, VII White/closure. NATIVE realms remain Phoenix Orange, Kitsune Green, Dragon Red, Unicorn Violet, Primordial Yellow, Leviathan Blue. Document supersession rather than deleting historical version.
7. Include `visuals/current/BLACK_PHOENIX_INTERNAL_NEON_3X3_EXPLORATORY.png` as exploratory visual, not definitive species canon; preserve old images. Store uploaded ELDRIS source PDF as a provenance reference in an appropriate source directory (e.g. `provenance/sources/ELDRIS_MASTER_UPLOADED_2026-10-10.pdf`), without altering its contents.
8. Preserve OPEN vs PROPOSED vs ESTABLISHED distinctions; all numerical realm-time examples are illustrative, NOT fixed canon. Preserve current source boundaries, `vaelum` institutional nuance, and no automatic old MK157 plot imports.
9. Produce `provenance/SEMANTIC_RECONCILIATION_v1.1.md` mapping **each decision** in the five update files to exact final repo file path and section, with statuses: integrated, already present, superseded, conflict, open. Check that all 5 files are accounted for. Record any unresolved conflict, do not invent a resolution.
10. Update current release metadata/README/AGENTS as appropriate; ensure no stale 'NOT_PUSHED' status after successful publication. Maintain historic archives.
11. Validate markdown links, source references, root constitution, all visual/source assets, no `_inbox` in Git. Commit and **push normally** to `main`; no force-push. Return commit SHA, changed files, and any unresolved semantic omissions. If permissions fail, explain precisely; do not claim success.

## Non-goals
Do not create a new repository, force-push, erase existing canon, invent story chapters or temporal ratios, or add unapproved rank multipliers.

## Package inventory clarification

The actual v1.1 ZIP contains four topical `updates/*.md` files plus the cumulative root constitution. The references above to five update files are a package count mismatch. Account for all four chapters and Part D; do not invent a fifth chapter. Incoming files are retained under `provenance/releases/v1.1.0/`.
