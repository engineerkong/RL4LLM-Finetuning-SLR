# Methodological Innovations in Reinforcement Learning for LLM Fine-Tuning: A Systematic Literature Review

This repository contains the worksheets behind the review:
- the Scopus search records with their screening and eligibility decisions,
- the data extracted from the 402 included papers,
- the coding of application tasks, addressed challenges and limitations,
- the recall check against three related surveys.

Each count, percentage and table in the paper can be traced to one of the sheets listed below.

## Review at a glance

| Stage | Papers |
|---|---:|
| Records identified in Scopus (2022–2025) | 4,552 |
| Excluded at title/abstract screening | 3,661 |
| Assessed for eligibility on full text | 891 |
| Excluded at eligibility | 489 |
| **Included** | **402** |

The included papers fall into three method domains:

| Domain | Abbreviation | Papers |
|---|---|---:|
| Fine-Tuning Algorithm | FA | 193 |
| Learning Framework | LF | 88 |
| Reward Modeling | RM | 121 |

## 📁 Worksheet Files

### 📋 RL4LLM_PRISMA_screening_eligibility_4552.xlsx

Search records and selection decisions (Section 2, Figure 2, Table 1, Appendix B).

| Sheet | Contents |
|---|---|
| Summary | PRISMA flow counts, computed by formulas over the other three sheets |
| 1 Records (4552) | The Scopus export: bibliographic data and abstract of every record, with its screening, eligibility and final decision |
| 2 After screening | Screening result for each record, with the failed criterion (Relevance, RL4LLM or Methodological development), the RL/LLM taxonomy sub-category and the reason |
| 3 After eligibility | Eligibility result for the 891 records that passed screening, with the failed criterion, the sub-reason (Table 1) and the reason |

### 📈 analysis_results_402.xlsx

The main analysis worksheet: data extracted from the 402 included papers (Sections 3 and 4).

| Sheet | Contents |
|---|---|
| #Algorithm, #Framework, #Reward | One row per paper in the FA, LF and RM domains (see below) |
| Section 3.1 counts | Formulas that compute the domain shares, application tasks, addressed challenges and method properties reported in Section 3.1 (Figures 3–5) |
| Task-challenge codes | Application-task and challenge codes for each paper, copied from `coding_tasks_challenges_402.xlsx` |
| Recent paradigms | Inclusion rules and paper lists for the recent paradigms discussed in Section 4: GRPO, process reward models and verifiers, verifiable rewards, and test-time compute |

Each row of the #Algorithm, #Framework and #Reward sheets gives:
- the primary method classification (domain → category → class; Tables 4–6),
- an optional secondary classification (Appendix A, Table 12),
- the answers to the extraction questions of Table 2: A.1–A.6 (RQ1), B.1–B.6 (RQ2) and C.1–C.2 (RQ3),
- the Scopus record ID.

### 🏷️ coding_tasks_challenges_402.xlsx

Coding of extraction answers A.2 (application tasks) and A.3 (addressed challenges) (Section 3.1, Figures 3 and 4).

| Sheet | Contents |
|---|---|
| Coding | For each paper, the A.2 and A.3 answers coded into 11 task and 11 challenge categories (multi-label, one 0/1 column per category) |
| Percentages | Share of papers in each domain that address each category |
| Codebook | Category definitions and coding rules |

### 🏷️ coding_limitations_402.xlsx

Coding of extraction answers C.1 (limitations) and C.2 (future directions) (Section 3.3, Figure 9, Tables 7–9).

| Sheet | Contents |
|---|---|
| Coding | For each paper, the C.1 and C.2 answers coded into 16 limitation types (multi-label, one 0/1 column per type), with future-direction codes |
| Percentages | Share of papers in each domain that report each limitation type |
| Codebook | Limitation definitions and coding rules |

### 🔍 recall_seed_set_three_surveys.xlsx

Recall of the search against a seed set drawn from the reference lists of three related surveys (Appendix A, Tables 10 and 11).

| Sheet | Contents |
|---|---|
| Summary | Steps from 1,124 reference entries to the 41-paper seed set, and the recall (37/41 = 90.2%, 95% Wilson CI 77.5–96.1%) |
| Seed set | Seed-set papers: 37 in the corpus, 4 missed, and the papers removed because their proceedings were not yet fully indexed by Scopus |
| All references | The unique references from the three surveys, each with its status: in the corpus, retrieved but excluded, not retrieved, or duplicate |
| Four missed papers | Extraction answers for the four missed papers (Table 11); these papers are not part of the review corpus |

### 🗄️ archive/

Earlier versions of the worksheets (November 2025 and March 2026), superseded by the files above:
- `screening_records_*.xlsx`: search and screening records
- `extraction_information_*.xlsx`: extraction answers by authors and LLMs
- `analysis_results_*.xlsx`: analysis results

## License

Released under the Apache License 2.0; see [LICENSE](LICENSE).
