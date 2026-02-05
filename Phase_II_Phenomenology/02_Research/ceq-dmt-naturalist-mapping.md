---
date: 25.09.01
time: 07:05:47
tags:
  - phenomenology
  - psychedelicResearch
---
# Psychedelic Phenomenology — CEQ + DMT Naturalistic + mapping

## CEQ — Challenging Experience Questionnaire — 26 Items (0–5 scale)

> These are the stand-alone CEQ items as per Supplementary Appendix 1 (Barrett et al., 2016):

- [ ] 1. I felt **frightened**.
- [ ] 2. I felt **panic**.
- [ ] 3. I felt **a sense that something terrible was about to happen**.
- [ ] 4. I felt **a sense of complete despair** or grief.
- [ ] 5. I felt **deep sadness**.
- [ ] 6. I felt **like crying**.
- [ ] 7. I felt **insane** or like I was losing control of my mind.
- [ ] 8. I felt **my mind was going crazy**.
- [ ] 9. I felt **like I might die**.
- [ ] 10. I felt **I was going to die**.
- [ ] 11. I felt **deeply alienated from everything**.
- [ ] 12. I felt **completely isolated**.
- [ ] 13. I experienced **physical pain**.
- [ ] 14. I experienced **nausea or stomach discomfort**.
- [ ] 15. I felt **my heart was racing or pounding**.
- [ ] 16. I experienced **chills or shivering**.
- [ ] 17. I experienced **feeling out of control of my body**.
- [ ] 18. I felt **paranoid**.
- [ ] 19. I felt **that people were plotting against me**.
- [ ] 20. I felt **antagonism from people around me**.
- [ ] 21. I experienced **terror**.
- [ ] 22. I felt **emotional suffering**.
- [ ] 23. I felt **psychological distress**.
- [ ] 24. I felt **extreme discomfort**.
- [ ] 25. I felt **like I was having a breakdown**.
- [ ] 26. I felt **absolutely out of my mind**.

**Subscale (factor) mapping — tag suggestions**:

| CEQ Item Numbers | Factor            | Suggested Tag           |
| ---------------- | ----------------- | ----------------------- |
| 1–4, 21          | Fear              | `#CEQ/Fear`             |
| 5–6, 22          | Grief             | `#CEQ/Grief`            |
| 7–8, 25–26       | Insanity          | `#CEQ/Insanity`         |
| 9–10             | Death             | `#CEQ/Death`            |
| 11–12            | Isolation         | `#CEQ/Isolation`        |
| 13–17, 23–24     | Physical Distress | `#CEQ/PhysicalDistress` |
| 18–20            | Paranoia          | `#CEQ/Paranoia`         |

---

## Naturalistic Inhaled DMT — Thematic Frequencies (Lawrence et al., 2022)

> These categories were coded thematically and percentage frequencies are from n = 3,778 unique experiences (3305 Reddit posts) :contentReference[oaicite:2]{index=2}:

- **Visual patterns (fractals, shapes, patterns):** 32.6%  
- **Vivid colours:** 25.2%  
- **Entity encounters:** reported in 45.5% of experiences, of which entity **types/phenotypes** include:
  - Feminine phenotype: 24.2%
  - Deities: 17.0%
  - Aliens: 16.3%
  - Creature-based (e.g. reptilian/insectoid): 9.2%
  - Mythological beings (including “machine elves”): 8.4%
  - Jesters: 6.5%
- **Entity interactions (valence/type):**
  - Positive/benevolent/comforting/protecting: 34.9% of encounters
  - Companion/pedagogical/guide-type: 32.4% of encounters
- **Architectural/features of the “DMT world”:**
  - Alternate/higher dimensions: 25.2%
  - Rooms (including “waiting room”): 15.4% (waiting room = 2.8%)
  - Tunnel: 10.3%
- **Statements of profundity (e.g., calling it “most beautiful experience”):** 6.1%  
  - Of these, “most beautiful of my life”: 1.2%

---

## Mapping Guide — RFN/MLFM Tag Strategy (Obsidian Import)

### Suggested Tag namespace proposal:

- **Visual layer**:
  - `#DMT/visual::fractals`, `#DMT/visual::patterns`, `#DMT/visual::vivid-colours`

- **Agent/entity layer**:
  - `#DMT/entity::feminine`, `#DMT/entity::deity`, `#DMT/entity::alien`, `#DMT/entity::creature`, `#DMT/entity::mythological`, `#DMT/entity::jester`
  - Interaction valence/type: `#DMT/entity-interaction::positive`, `#DMT/entity-interaction::companion-guide`

- **Spatial/architectural layer**:
  - `#DMT/env::higher-dimension`, `#DMT/env::room`, `#DMT/env::waiting-room`, `#DMT/env::tunnel`
  
- **Profundity layer**:
  - `#DMT/statement::profundity`, `#DMT/statement::most-beautiful`

### Use frequency-based weighting (e.g., in CSV or modeling):

| Category                          | Frequency (%) | Weight Suggestion     |
|-----------------------------------|---------------|------------------------|
| Visual – fractals/patterns        | 32.6          | Medium-high baseline  |
| Visual – vivid colours            | 25.2          | Medium baseline       |
| Entity encounter overall          | 45.5          | High baseline         |
| Entity – feminine                 | 24.2          | Moderate              |
| Deity                             | 17.0          | Moderate              |
| Alien                             | 16.3          | Moderate              |
| Creature-based                    | 9.2           | Low-medium            |
| Mythological (machine elves)      | 8.4           | Low-medium            |
| Jester                            | 6.5           | Low                   |
| Entity-positive interaction       | 34.9          | Medium-high           |
| Companion/guide interaction       | 32.4          | Medium-high           |
| Env – higher dimensions           | 25.2          | Medium baseline       |
| Env – room                        | 15.4          | Low-medium            |
| Env – waiting-room                | 2.8           | Low                   |
| Env – tunnel                      | 10.3          | Low-medium            |
| Profundity                        | 6.1           | Low-medium            |
| “Most beautiful life”             | 1.2           | Very low              |

---
##### Sources:
  - Barrett et al., 2016 — CEQ Supplementary Appendix 1 (stand-alone 26 items) :contentReference[oaicite:0]{index=0}  
  - Lawrence et al., 2022 — Naturalistic inhaled DMT thematic frequencies (Scientific Reports) :contentReference[oaicite:1]{index=1}

---
