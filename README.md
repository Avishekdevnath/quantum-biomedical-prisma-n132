# PRISMA 2020 Master Evidence Ledger & 4-Vector Risk-of-Bias Dataset ($n = 132$)

This repository hosts the curated machine-readable dataset accompanying the review manuscript:

> **Quantum-Enhanced Molecular Intelligence in Biomedical Engineering: A Comprehensive Review of AI-Driven Diagnostics, Drug Discovery, and Scalable Quantum Computing**  
> **Authors:** Prof. Dr. Hafiz Md. Hasan Babu (Senior Member, IEEE; [ORCID: 0009-0003-2507-0400](https://orcid.org/0009-0003-2507-0400)) and Avishek Devnath ([ORCID: 0009-0000-2779-6713](https://orcid.org/0009-0000-2779-6713))  
> **Affiliation:** Department of Computer Science and Engineering, University of Dhaka, Dhaka 1000, Bangladesh  
> **Target Venue:** *IEEE Reviews in Biomedical Engineering* (RBME)

---

## Dataset Overview

- **File:** `master_prisma_n132_benchmarks.csv`
- **Total Verified Studies:** $n = 132$ peer-reviewed empirical studies (2014–2026; zero unrefereed preprints)
- **Domain Pillars:**
  - `VQA` — Variational Quantum Algorithms & Chemistry ($n = 61$)
  - `QML` — Quantum Machine Learning & Clinical Diagnostics ($n = 27$)
  - `DOCK` — Combinatorial Docking & Protein Folding ($n = 23$)
  - `OPEN` — Open Quantum Molecular & Biological Dynamics ($n = 21$)
- **Full-Text Audit Coverage:** 80 Open-Access Full-Text XML (`OA Full-Text XML`), 52 Verified Metadata/Abstract (`Verified Metadata/Abstract`)
- **Execution Mode Breakdown:** 58 Physical QPU (`51 Physical QPU + Emulator`, `7 Physical QPU`), `34 Ideal Emulator`, `33 Noisy Emulator`, `4 Unspecified`, `3 FTQC Resource Est.`

---

## Schema (`master_prisma_n132_benchmarks.csv`)

| Column | Description |
|---|---|
| `Study_ID` | Unique identifier within the curated PRISMA corpus (`S001`–`S132`) |
| `Year` | Publication year (2014–2026) |
| `Pillar` | Research pillar (`VQA`, `QML`, `DOCK`, or `OPEN`) |
| `First_Author_Citation` | First author and publication year label |
| `Journal` | Peer-reviewed journal or proceedings venue |
| `DOI` | Digital Object Identifier (resolvable via `https://doi.org/<DOI>`) |
| `PMID` | PubMed ID (where indexed) |
| `PMCID` | PubMed Central ID (where indexed for Open-Access XML) |
| `Title` | Full article title |
| `FullText_Audited` | Audit depth (`OA Full-Text XML` vs `Verified Metadata/Abstract`) |
| `Hardware_or_Simulator` | Reported quantum processor or software simulator platform |
| `Execution_Mode` | Execution classification (Physical QPU, Noisy/Ideal Emulator, FTQC Resource Est.) |
| `Qubits_Reported` | Number of physical or logical qubits reported |
| `Error_Mitigation` | Quantum error mitigation or error correction protocol reported |
| `Shots_Reported` | Measurement shot budget reported |
| `Classical_Baselines` | Head-to-head classical HPC/AI baselines benchmarked |
| `Primary_Outcome_Snippet` | Audited primary quantitative finding |
| `RoB1_Hardware_Realism` | Risk-of-Bias Vector 1 (Hardware Realism) |
| `RoB2_Protocol_Integrity` | Risk-of-Bias Vector 2 (Protocol Integrity) |
| `RoB3_Baseline_Parity` | Risk-of-Bias Vector 3 (Classical Baseline Parity) |
| `RoB4_Shot_Runtime_Transparency` | Risk-of-Bias Vector 4 (Shot & Runtime Transparency) |
| `Overall_RoB_High_Count` | Count of high-risk-of-bias vectors per study (0–4) |

---

## License

This dataset is shared under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license. See [LICENSE](LICENSE) for details.
