# MK231 v1.1 semantic reconciliation — 2026-10-10

## Baseline and method

Local worktree was clean on main; fetch confirmed live origin/main at `61c15595454360757e947a7fda0e7b95b8d98d2d`, with no newer commits. Compared incoming substantive decisions against canon, story, current synthesis, specialized constitutions, source/decision/asset ledgers, README, AGENTS and state metadata. Existing root constitution was absent: the previous restore run made no edits because the initial ZIP lacked it. No concurrent restoration work was overwritten.

All 10 supplied SHA-256 entries and manifest byte counts passed before integration. Exact incoming payload retained under `provenance/releases/v1.1.0/`; the initial release manifest/checksums/runbook/cumulative reading copy are retained under `provenance/releases/v1.0.0/`. Current synthesized sections are refreshed from their owning documents; the historical appendix and all historical files are preserved. Former labels and ambiguity are retained as explicitly superseded records. No upstream plots or speculative timing values became canon.

## Decision-to-destination reverse diff

Statuses describe reconciliation: **integrated**, **already present**, **superseded**, **conflict**, **open**. Superseded marks the previous mapping replaced by explicit approval. Open retains deliberate OPEN/PROPOSED/illustrative limitations. Paths and section titles are exact; CURRENT_LIVE_MODEL.md mirrors those source sections, plus the root constitution in Section R.

| ID | Incoming file | Decision | Status | Final path and section |
|---|---|---|---|---|
| 11-01 | 01_STACK_AND_BOOKS.md | L0 mathematical/physical reference; exclude computer architecture | integrated | canon/00_THE_STACK_AND_BOUNDARIES.md — v1.1 — Five-layer author/world framework (ESTABLISHED) |
| 11-02 | 01_STACK_AND_BOOKS.md | L1 fantasy engine, L3 independent character engine, L4 causal narrative | already present | canon/00_THE_STACK_AND_BOUNDARIES.md — v1.1 — Five-layer author/world framework (ESTABLISHED) |
| 11-03 | 01_STACK_AND_BOOKS.md | L2 environmental plus civilization engines; romanticized preindustrial White and engineered stone blocks | integrated | canon/00_THE_STACK_AND_BOUNDARIES.md — v1.1 — Five-layer author/world framework (ESTABLISHED); canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — MK147 societal inheritance |
| 11-04 | 01_STACK_AND_BOOKS.md | Reusable author framework, not in-world ranks | integrated | canon/00_THE_STACK_AND_BOUNDARIES.md — v1.1 — Five-layer author/world framework (ESTABLISHED) |
| 11-05 | 01_STACK_AND_BOOKS.md | _bricked L0, MK147 L1/L2, selective MK157, original MK231; no wholesale clones or old plots | integrated | canon/00_THE_STACK_AND_BOUNDARIES.md — v1.1 — Source boundaries; provenance/SOURCE_MAP.md — v1.1 author-approved selective inheritance — 2026-10-10 |
| 11-06 | 01_STACK_AND_BOOKS.md | Book labels I Red, II Orange, III Yellow, IV Green, V Blue, VI Violet, VII White | superseded | story/03_SEVEN_BOOKS_AND_COMPANIONS.md — opening book table; v1.1 — Book labels and native realms (ESTABLISHED) |
| 11-07 | 01_STACK_AND_BOOKS.md | Companion acquisition and Orange/Green/Red/Violet/Yellow/Blue native identities unchanged | already present | story/03_SEVEN_BOOKS_AND_COMPANIONS.md — Acquisition pattern; v1.1 — Book labels and native realms (ESTABLISHED) |
| 11-08 | 01_STACK_AND_BOOKS.md | Book I starts in White; Orange visit may follow; never Red-native Phoenix | integrated | story/04_BOOK_ONE_EVENT_SCAFFOLD.md — v1.1 — Book I Red / Phoenix Orange |
| 11-09 | 02_PROPHECY_TIME_AND_BINDINGS.md | Prophecies concern magic itself, Seven Realms existence structure, Black [0,1] union | already present | canon/02_EIGHT_PROPHECIES_OF_MAGIC.md — v1.1 — Black Prophecy and interpretation |
| 11-10 | 02_PROPHECY_TIME_AND_BINDINGS.md | Vague heal existence reference; ending monster threat is consequence, not extermination mandate | integrated | story/02_THE_BLACK_PROPHECY.md — v1.1 — Black Prophecy |
| 11-11 | 02_PROPHECY_TIME_AND_BINDINGS.md | Unicorn keepers interpret more deeply and guide Kira; ancient verses OPEN | integrated | canon/02_EIGHT_PROPHECIES_OF_MAGIC.md — v1.1 — Black Prophecy and interpretation |
| 11-12 | 02_PROPHECY_TIME_AND_BINDINGS.md | Explicitly selected high/displaced Yellow-neon instability contributes to collapse, storms, ELDRIS | integrated | canon/01_COSMOLOGY_AND_SPECTRUM.md — v1.1 — Selected Yellow-neon anomaly and restoration |
| 11-13 | 02_PROPHECY_TIME_AND_BINDINGS.md | Exact neon numbers, root cause and repair operator OPEN; no old MK157 resolution scene | open | canon/01_COSMOLOGY_AND_SPECTRUM.md — v1.1 — Selected Yellow-neon anomaly and restoration |
| 11-14 | 02_PROPHECY_TIME_AND_BINDINGS.md | Energy-combined egg, unicorn prophecy, theft/loss, contact relief, therapeutic attempt, independent hatch and further emergence | already present | story/02_THE_BLACK_PROPHECY.md — v1.1 — First Binding and emergence |
| 11-15 | 02_PROPHECY_TIME_AND_BINDINGS.md | After first Binding only Black shared-existence Bindings; no ordinary shaping Bindings | already present | story/02_THE_BLACK_PROPHECY.md — v1.1 — First Binding and emergence |
| 11-16 | 02_PROPHECY_TIME_AND_BINDINGS.md | Three eggs, lattice cradle, two conscious voluntary agreements; guardianship/trust/service | integrated | story/02_THE_BLACK_PROPHECY.md — v1.1 — First Binding and emergence |
| 11-17 | 02_PROPHECY_TIME_AND_BINDINGS.md | Dragon war and Kirati label remain proposed | open | story/02_THE_BLACK_PROPHECY.md — v1.1 — First Binding and emergence (PROPOSED) |
| 11-18 | 02_PROPHECY_TIME_AND_BINDINGS.md | Reciprocal companion amplification and selected Kira capability; not conventional Augmenter | integrated | canon/03_TRANSDUCTION_VAEN_BINDINGS.md — v1.1 — Reciprocal universal amplification |
| 11-19 | 02_PROPHECY_TIME_AND_BINDINGS.md | Violet-comparable Phoenix is illustrative, not native/rank/multiplier change; amplification limits OPEN | open | canon/03_TRANSDUCTION_VAEN_BINDINGS.md — v1.1 — Reciprocal universal amplification |
| 11-20 | 02_PROPHECY_TIME_AND_BINDINGS.md | Independent coherent realm histories, linear personal narrative, continued evolution, pre-encounter Black histories | integrated | workshop/CHRONOLOGY_NARRATIVE_OPEN.md — v1.1 — Independent realm clocks |
| 11-21 | 02_PROPHECY_TIME_AND_BINDINGS.md | No shared clock/fixed ratio; age 27, four years, egg 200, Kitsune 15–25, 57 and 3/7/1.7/200 examples illustrative; causality OPEN | open | canon/01_COSMOLOGY_AND_SPECTRUM.md — v1.1 — Independent realm clocks |
| 11-22 | 02_PROPHECY_TIME_AND_BINDINGS.md | Community interpretations, diplomacy/service; unicorn guidance/shared purpose/consent; conflicts OPEN | integrated | story/03_SEVEN_BOOKS_AND_COMPANIONS.md — v1.1 — Story-level consequences |
| 11-23 | 03_BOOK_ONE_BLACK_PHOENIX.md | Age 23 adopted Afflicted smith, 11–17/37 mortality, savings/prior economic restriction, temporary contact relief | already present | story/01_KIRA_AND_AFFLICTION.md — v1.1 — Starting condition and post-Binding limit |
| 11-24 | 03_BOOK_ONE_BLACK_PHOENIX.md | Full post-Binding genetic outcome OPEN | open | story/01_KIRA_AND_AFFLICTION.md — v1.1 — Starting condition and post-Binding limit |
| 11-25 | 03_BOOK_ONE_BLACK_PHOENIX.md | Hawk/fire-hawk entirely dynamic BLACK FLAME, six internal changing neon channels, no feathers/exterior rainbow/fixed stripes | integrated | canon/05_NATIVE_RACE_MAGIC.md — v1.1 — Black Phoenix visual reference |
| 11-26 | 03_BOOK_ONE_BLACK_PHOENIX.md | Later humanoid timing OPEN; 3×3 concept exploratory, not locked physiology | open | canon/05_NATIVE_RACE_MAGIC.md — v1.1 — Black Phoenix visual reference |
| 11-27 | 03_BOOK_ONE_BLACK_PHOENIX.md | Phoenix exceptional Coherence/native rebirth and Kira exceptional Decoherence; complementary amplified Persistent Topology | integrated | canon/03_TRANSDUCTION_VAEN_BINDINGS.md — v1.1 — Complementary Persistent Topology |
| 11-28 | 03_BOOK_ONE_BLACK_PHOENIX.md | Ordinary Decoherence weak/inefficient; stabilization easier; Kira can target recursive ELDRIS closure without guaranteed victory | integrated | canon/03_TRANSDUCTION_VAEN_BINDINGS.md — v1.1 — Complementary Persistent Topology |
| 11-29 | 03_BOOK_ONE_BLACK_PHOENIX.md | Kira extraordinary lowercase helkir, not conventional Summoner; personal rebirth/fatigue/targeting/resistance/scale/range OPEN | open | canon/03_TRANSDUCTION_VAEN_BINDINGS.md — v1.1 — Complementary Persistent Topology |
| 11-30 | 03_BOOK_ONE_BLACK_PHOENIX.md | White Book I dungeon aithren toolkit, possible later Orange; no Kitsune until II Orange/native Green; Resolution/Bandwidth/Chirality mechanism OPEN | integrated | story/04_BOOK_ONE_EVENT_SCAFFOLD.md — v1.1 — Book I Red / Phoenix Orange |
| 11-31 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Five professions and associations; social classifications, not fundamental magical divisions | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — Human professions |
| 11-32 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Architect velis direct temporary topology, distinct physical ru’ne/sigils; long low-load life, attrition and maintenance | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — Architects and agriculture |
| 11-33 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Suitable-crop seven harvests with enriched soil, not universal; mostly vegetarian, risky livestock; MK147 17×13 taxonomy | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — Architects and agriculture |
| 11-34 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Uploaded source and selective inherited ELDRIS: bounded runaway recursive collapse, black roots/wisps, basin leakage, not Black Kira/evil/dungeon-only | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — ELDRIS |
| 11-35 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Six basin ELDRIS expressions; broad A R/O/Y, B G/B, C V threat categories, not universal ranks; storms possible | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — ELDRIS |
| 11-36 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Persistent mapped R→V dungeons, compatible containment, stable settlements, changeable configurations, never permanently cleared | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — Dungeons and domai |
| 11-37 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Storm not automatically domai; bounded non-isometric R→V event, White non-conscious core, unraveling/resources, response distinctions, no Valnak rules | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — Dungeons and domai |
| 11-38 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | aithren participatory values, delvers/support towns and mobile storm chasers/logistics; overlap permitted | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — `aithren` cultural identity |
| 11-39 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Engineer/NASCAR/FOB/tornado analogies only, no technology import; ER Foam social information exchange | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — `aithren` cultural identity |
| 11-40 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Independent recognized contract-capable vaelum; Crown/Accord recognition not centralized military command | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — `vaelum` and Accord Registry |
| 11-41 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | All named contract categories and qualifying tax/property/housing benefits, exact rates/scoring OPEN; exclude ELN/Highway/Heart/Chimera/payout imports | integrated | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — `vaelum` and Accord Registry |
| 11-42 | 04_WORLD_AITHREN_VAELUM_ELDRIS.md | Age of Knowledge/Chainmail Robe historical upstream, not Kira chronology | already present | canon/07_WORLDBUILDING_CULTURE_GEOGRAPHY.md — Source boundaries |
| 11-43 | CONSTITUTION.md Part D | MK231 is a five-layer reusable high-fantasy framework; all paragraphs retained | integrated | CONSTITUTION.md — MK231 is a five-layer reusable high-fantasy framework |
| 11-44 | CONSTITUTION.md Part D | Source authority and non-cloning; all paragraphs retained | integrated | CONSTITUTION.md — Source authority and non-cloning |
| 11-45 | CONSTITUTION.md Part D | Two different color sequences — do not confuse; all paragraphs retained | integrated | CONSTITUTION.md — Two different color sequences — do not confuse |
| 11-46 | CONSTITUTION.md Part D | Independent realm time; all paragraphs retained | integrated | CONSTITUTION.md — Independent realm time |
| 11-47 | CONSTITUTION.md Part D | Kira's Black Binding / power progression; all paragraphs retained | integrated | CONSTITUTION.md — Kira's Black Binding / power progression |
| 11-48 | CONSTITUTION.md Part D | Black Prophecy and cosmological restoration; all paragraphs retained | integrated | CONSTITUTION.md — Black Prophecy and cosmological restoration |
| 11-49 | CONSTITUTION.md Part D | Civilization / aithren; all paragraphs retained | integrated | CONSTITUTION.md — Civilization / aithren |
| 11-50 | CONSTITUTION.md Part D | Release safety; all paragraphs retained | integrated | CONSTITUTION.md — Release safety |
| 11-51 | CONSTITUTION.md Parts A–C | Complete portable aggregate, source preservation, statuses, named-character and presentation discipline, lower-case terms and independent specialized maintenance | integrated | CONSTITUTION.md — Parts A–C; README.md — Critical starting points; AGENTS.md — opening instructions |

## Root constitution reconciliation

Incoming root SHA-256 is `eecffcd80bb53d6129262fd6cc61c4832e5fe4bf8805032b08163195ed92494c`; its exact bytes are retained in the release payload. No existing root file was available to merge. All incoming Parts A–D are retained; root release date/version and primary-portable designation were updated, its chromatic-reference path corrected, and Parts A–C synchronized with the three retained specialized files, including approved portable-release policies and book-label presentation clarification. The earlier requested v1.0 hash `e592d9207a16c6c4023be3871a4a2916a3a6a63947ab7424e8cc9d225cc90175` is not claimed for this updated version. Its original source remains unavailable.

## Unresolved information gaps and intentional OPEN limits

- Runbook step 9 says five update files; ZIP and manifest contain **four** topical updates. All four and every Part D subsection are mapped above (51 decision rows). No fifth topical file was supplied; its existence/content cannot be inferred.
- Upstream precise paths for the newly supplied civilization/ELDRIS details are not all provided. The exact uploaded PDF and author-approved update chapters are retained as evidence. This run does not claim a fresh exhaustive audit of MK147/MK157/_bricked or verification of every PDF assertion.
- Exact Yellow displacement/root/repair; ancient verses; realm-clock correspondences/causality; amplification limits; Kira rebirth and post-Binding genetics; combat constraints; humanoid timing; specific later conflicts and vaelum benefit rates remain OPEN. Dragon war/Kirati are PROPOSED. Numerical time and capability examples remain illustrative.
- No unresolved contradictory author decisions block integration. The prior book-color lock and final-companion swap ambiguity are explicitly superseded by v1.1 while native realms and acquisition order are preserved.

## Verification and publication evidence

Current `bundle_manifest.json` and `SHA256SUMS.txt` cover reconciled release contents; the original manifests are retained as evidence. `scripts/verify_bundle.py` checks current hashes/lengths, exact archival extraction, mandatory root constitution and new assets, excludes local inbox/Git/staging, and rejects unexpected committed-content files. Markdown local links are checked against existing targets. A clean staged export is verified before commit; remote SHA equality and root-constitution accessibility are checked after normal push. Publication evidence is the Git commit containing this report, reported by Codex after push; no self-referential commit hash is fabricated here.
