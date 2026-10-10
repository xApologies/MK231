# Executable.md — MK231 cumulative bootstrap and GitHub publication

**For Codex, acting at the author's direction.** The author has placed this cumulative ZIP in a Windows local `_inbox` folder and wants its *contents* organized as the first full model of an existing GitHub repository: `https://github.com/xApologies/MK231`.

**Execution target:** Populate and publish **the existing `xApologies/MK231` repo**. Do not make a second GitHub repository. Its GitHub repository already existed and appeared empty during ZIP preparation; verify live state at run time. Do not create a new project folder with a similar name (`MK31`, `MK147`, `MK157`, etc.). The correct name is `MK231`.

## Primary invariants

1. The author's Windows project directory is `%USERPROFILE%\MK231\`. Locate it rather than guessing the actual Windows account name.
2. `%USERPROFILE%\MK231\_inbox\` is a **local-only ingestion/drop folder**. Keep the ZIP there for the author's records. Never upload, track, relocate or delete `_inbox` or its contents as part of the Git commit. `.gitignore` contains the exclusions; explicitly **verify** them.
3. Every ZIP top-level path maps directly to the **repository root**. `Executable.md` must be in repo root; do **not** nest the repository under a second `MK231/` folder.
4. Prior full live model v0.3.0 files under `history/v0.3.0/` are immutable source history. The exact original ZIP under `provenance/` is intentionally preserved. Do not lose pictures, ancient archive, naming conventions, constitution PDF/DOCX, source ledgers or any current delta.
5. All assistant/user-provided exploratory imagery remains `VISUAL REFERENCE`, not finalized physical design unless an explicit selection says otherwise. No auto-filled seventh Leviathan, premature prophecy wording or unapproved cosmological theorem.
6. This instruction file is a human-readable execution plan, **not** an operating-system executable. Follow the checks below and stop for collisions/errors.

## Runbook

### 1. Discover and audit

- Confirm the current working directory resolves to the author's `MK231` project directory and contains `_inbox` (or ask which directory if different).
- Check Git auth, `git status`, `git remote -v`, `git branch -avv`, and the existence/content of `https://github.com/xApologies/MK231`. Verify repo owner, remote and branch; expected default is `main`.
- If **existing committed work or uncommitted author files** are present, **DO NOT REPLACE THEM**. Report differences, stage on a distinct working branch or backup safely, and reconcile with author before destructive operations. The current ZIP is a baseline only if destination is empty/new.
- Find the latest `MK231_FULL_CUMULATIVE_LIVE_MODEL_v1.0.0.zip` in `_inbox`; if multiple candidate ZIPs exist, select by the specified filename rather than modification time. Validate archive entries (no absolute paths, no `..`, no `.git`, no `_inbox`).

### 2. Safe extraction

- Create temporary `MK231\.mk231_staging\v1.0.0\` (ignored by `.gitignore`).
- Extract the archive **there** and verify `Executable.md`, `README.md`, `AGENTS.md`, `CURRENT_LIVE_MODEL.md`, `canon/`, `story/`, `constitution/`, `provenance/`, `history/v0.3.0/`, and `visuals/` are present.
- Run `python scripts/verify_bundle.py` from the extracted staging root to check file hashes, manifest and the archival cumulative files. If Python isn't available, verify SHA-256 checksums against `SHA256SUMS.txt` or use PowerShell `Get-FileHash`.
- Transfer only staged repository-root content (NOT the staging directory itself) into the MK231 working root. Do not copy `_inbox` or overwrite unrelated pre-existing author files. Keep the original ZIP in `_inbox`.
- When convenient, retain the temporary staging copy until validation and Git publication succeed; then clean only this staging copy (not the original ZIP).

**PowerShell example** (run inside project root only after setting exact ZIP path):

```powershell
$repo = Join-Path $env:USERPROFILE 'MK231'
$zip  = Join-Path $repo '_inbox\MK231_FULL_CUMULATIVE_LIVE_MODEL_v1.0.0.zip'
$stage = Join-Path $repo '.mk231_staging\v1.0.0'
if (-not (Test-Path -LiteralPath $zip)) { throw "Archive missing: $zip" }
New-Item -ItemType Directory -Force -Path $stage | Out-Null
Expand-Archive -LiteralPath $zip -DestinationPath $stage -Force
python (Join-Path $stage 'scripts\verify_bundle.py') --root $stage
# Inspect $stage, git state, and destination collisions BEFORE copying.
# Codex should then transfer staged files except .git and _inbox to $repo.
```

### 3. Initialize/preserve Git history

- If this is a true empty local project, initialize `git init -b main` (or compatible commands), attach `origin https://github.com/xApologies/MK231.git`, and fetch to detect a remote branch that may have appeared after ZIP preparation.
- If `main` already has history, preserve it and reconcile. **Never force-push, reset --hard, delete a branch, or overwrite commits**.
- Review additions as one cumulative bootstrap. `git status --short`; ensure expected files present and no old content missing.
- Confirm `_inbox` is ignored using `git check-ignore -v _inbox` and that staging is ignored. Verify no `_inbox` paths are tracked (`git ls-files` must not contain them). Verify ignored secrets are absent.
- Run `python scripts/verify_bundle.py --root .`. If the files were intentionally edited during reconciliation, refresh the manifest first and describe those changes; do not bypass verification silently.

### 4. Commit and push

- Stage only intended MK231 files, including original archive in `provenance` and all binary image references in `history` and `visuals/current`.
- Suggested commit message: `Bootstrap MK231 cumulative live model v1.0.0 — eight prophecies and Black Phoenix saga`.
- Push to the verified `origin/main` only if it is safe fast-forward and the current user authorizes the deployment (the author's present request authorizes the initial population of this repo). If a later remote change conflicts, stop and ask.
- Report the final commit SHA, branch, files committed, key paths, and that `_inbox` was **not** uploaded. Optionally compare hashes of current binary visuals and original v0.3.0 ZIP against `SHA256SUMS.txt`.

### 5. Ongoing authoring protocol

For future ZIP increments: place the ZIP in `_inbox`, unpack to a temporary staging area, read the internal `Executable.md`, compare with current Git HEAD, apply only approved deltas, update `CURRENT_LIVE_MODEL.md`, constitution/decision provenance as required, validate media, commit and push. Use Git as persistent authority. Never assume conversation memory equals a Git commit. The archived earlier models remain accessible for recovery.

## Canon checklist for this release (prevent source contamination)

- [ ] **Eight Prophecies**, including Seven Realms (not Six Realms) and Black as eighth; never seven schools inside the realms.
- [ ] Kira age **23**; typical Afflicted deaths **11–17**, oldest documented **37**; genetic condition, superstition not actual contagion.
- [ ] Low-income adopted armorsmith family saves for rare `vaen`/Genesis-crystal therapeutic Binding; Kira has no early ordinary Bindings because of resources.
- [ ] Black Phoenix egg energy-combination origin → unicorn speaks prophecy → theft/loss → White → Kira temporary hand relief → egg mistaken for useful vaen → exceptional identity Binding/hatch.
- [ ] Kira is Black manifestation of full `[0,1]` neon spectrum, White is actual chromatic superposition, no eighth basin, no literal limitless control.
- [ ] After first exceptional Binding Kira's new Bindings can only be with other **Black** existences; shared capabilities and independent consent preserve friend identities.
- [ ] Seven books **Orange / Green / Red / Violet / Yellow / Blue / White**, while late spoken alternate Leviathan-vs-Primordial order remains OPEN rather than silently revised.
- [ ] Six selected Leviathan types, **Fractal Spine #8** Horizon native visual; optional seventh not mandated; latest 2×3 female humanoid art exploratory.
- [ ] No MK147 or MK157 legacy story plots imported without current author permission.

## Expected result

A published `https://github.com/xApologies/MK231` working tree containing the full cumulative live model, narrative source files, chromatic workshopping constitution, source/history archive, images/gallery, decision ledger, and future-upgrade instructions. `_inbox` remains a local-only ZIP archive and is absent from remote Git history.
