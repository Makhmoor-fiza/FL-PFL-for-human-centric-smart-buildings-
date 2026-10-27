[README.md](https://github.com/user-attachments/files/33713278/README.md)
# From Federated Learning to Personalized Intelligence: A Systematic Review of Human-Centric Smart Buildings

`#PersonalizedFederatedLearning` `#FederatedLearning` `#SmartBuildings` `#HumanCentricAI` `#OccupantCentric` `#PrivacyPreservingLearning` `#EdgeIntelligence` `#SystematicReview` `#PRISMA`

## Authors

**Sundas Sarwar**, **Makhmoor Fiza Murk**, **Daniela Annunziata**, **Francesco Piccialli**\*

University of Naples Federico II, Department of Mathematics and Applications "R. Caccioppoli",
M.O.D.A.L. (Mathematical mOdelling and Data AnaLysis) research group, Naples, Italy

\* Corresponding author: francesco.piccialli@unina.it

## About this repository

This repository accompanies our systematic review of Federated Learning (FL) and Personalized Federated Learning (PFL) for human-centric smart buildings. It contains the articles retrieved in the initial literature search and the final set of studies selected after screening, to support the transparency and reproducibility of the review.

## Abstract

Personalized Federated Learning (PFL) is emerging as a promising paradigm for human-centric smart buildings, where collaborative intelligence must accommodate diverse occupant preferences, behaviors, building conditions, and resource capabilities while preserving data privacy. Although Federated Learning (FL) enables collaborative model training without centralizing raw data, a single global model may struggle with the statistical, system, and temporal heterogeneity inherent in real-world building environments. PFL addresses this limitation by adapting collaboratively learned knowledge to heterogeneous occupants, buildings, zones, and devices. However, personalization at the building or device level does not necessarily imply human-centric personalization, which requires explicit consideration of occupant preferences, comfort, behavior, feedback, or related human outcomes. This survey systematically analyzes 41 studies and develops an application-oriented taxonomy mapping FL and PFL approaches across five smart-building domains. We examine personalization targets and strategies, datasets, evaluation metrics, and benchmarking protocols, with particular attention to realism, reproducibility, and cross-study comparability. We further analyze how resource-constrained edge and IoT infrastructures affect communication, computation, latency, and practical PFL deployment, as well as the trade-off between personalization and privacy. The analysis identifies persistent challenges related to data scarcity, heterogeneity, cold-start adaptation, scalability, privacy, fairness, and explainability, and reveals an important distinction between occupant-centric personalization and approaches that primarily adapt models to buildings, zones, or devices. Based on these findings, we outline future directions toward data-efficient and continual personalization, resource-efficient edge intelligence, trustworthy privacy-preserving PFL, standardized real-world evaluation, and digital-twin-assisted personalized intelligence. Overall, this survey provides a structured foundation for advancing adaptive, privacy-aware, and genuinely occupant-centric intelligence in future smart buildings.

## Research questions

- **RQ1:** How are existing PFL paradigms and personalization strategies applied across human-centric smart-building applications?
- **RQ2:** Which datasets, experimental settings, and evaluation metrics are used to assess FL and PFL in smart buildings, and what limitations in data realism, reproducibility, and cross-study comparability characterize current evaluation practices?
- **RQ3:** How do resource-constrained edge environments and heterogeneous IoT infrastructures affect the communication, computation, memory, latency, and scalability of PFL deployment in smart buildings?
- **RQ4:** What trade-offs arise between personalization performance and privacy protection in distributed smart-building systems, and how should these trade-offs inform future privacy-preserving PFL research?

## Repository structure

| File | Description |
|---|---|
| `searched_papers.xlsx` | The 58 unique records retrieved from the five databases across both search rounds, after duplicate removal, which entered title and abstract screening |
| `selected_papers.xlsx` | The 41 primary studies included in the review after screening and full-text assessment |
| `PRISMA.png` | PRISMA flow diagram of the study-selection process |

Each spreadsheet lists the serial number, paper title, and publication year.

## Methodology

The review follows the PRISMA guidelines.

- **Databases:** Scopus, Web of Science, IEEE Xplore, ScienceDirect, and Semantic Scholar
- **Initial search:** June 24, 2026 (65 records)
- **Supplementary search:** September 15, 2026 (15 additional records), same databases, query, eligibility criteria and screening procedure
- **Final search cut-off:** September 15, 2026
- **Publication window:** 2017 onward (the earliest eligible studies were published in 2019)
- **Language:** English only
- **Search fields:** title, abstract, and keywords (where supported by the database)

**Boolean query** (syntax adapted to each database):

```
(("smart building" OR "intelligent building" OR "building energy management")
 AND ("personalized" OR "user-aware" OR "occupant-centric" OR "human-centric")
 AND ("federated learning" OR "personalized federated learning"))
```

The records from both search rounds (80 in total) were pooled and deduplicated before screening.

### PRISMA flow diagram

<p align="center">
  <img src="PRISMA.png" alt="PRISMA flow diagram of the study selection process" width="600">
</p>

## Application domains

The 41 included studies are grouped into five human-centric smart-building domains:

| Domain | Share of studies |
|---|---|
| Energy Intelligence | 31.7% |
| Thermal Comfort & Indoor Environmental Quality | 24.4% |
| Occupancy & Human Behavior Analytics | 24.4% |
| Edge Intelligence & IoT Infrastructure | 14.6% |
| Privacy-Preserving Personalization | 4.9% |

### Publication trend

| Year | 2019 | 2020 | 2021 | 2022 | 2023 | 2024 | 2025 | 2026 |
|---|---|---|---|---|---|---|---|---|
| Included studies | 2 | 1 | 1 | 1 | 5 | 6 | 13 | 12 |

Research activity has grown markedly since 2023, with most included studies published in 2025 and 2026.

## How to use this repository

- Browse `selected_papers.xlsx` for the curated list of FL/PFL studies on human-centric smart buildings.
- Use `searched_papers.xlsx` together with the search query above to replicate, audit, or extend the review.
- Reuse the curated list as a starting point for benchmarking, secondary studies, or related surveys.
