## Threat Hunters 1 — Attribution Analysis: Operation Digital Storm

### Project Overview
This project is part of the Attribution Techniques in Cyberwarfare assessment. Our objective is to perform a comprehensive attribution analysis of the case study “Operation Digital Storm,” a sophisticated attack on critical energy infrastructure.

“Operation Digital Storm” is a fictional scenario. To ensure analytical rigor and verifiable sourcing, we model evidence, TTPs, and infrastructure on the real 2015–2016 cyberattacks on Ukraine’s power grid commonly attributed to the Sandworm group (GRU Unit 74455). We clearly separate verifiable facts from analytical assessments and cite reputable sources.

### Key Objectives
- Analyze technical evidence (malware, infrastructure, TTPs).
- Correlate with non-technical indicators (geopolitical context, linguistic cues, targeting patterns).
- Compare findings against known APT groups and assess confidence.
- Provide strategic recommendations to improve attribution and defense.

### Team & Collaboration
- **Imtiyaz Ahmad:** Lead for Recommendations, Infrastructure Research, README compilation. Contributions: Threat Actor Comparison Matrix, code reuse, infrastructure tracing, diplomatic/economic context.
- **Yusuf Ibrahim Lawal:** Lead for Geopolitical Context,  TTP mapping. Contributions: malware families, OPSEC, motives/beneficiaries.
- **Laiba Waseem:** Support for malware indicators, certificate evidence, beneficiaries. Contributions: linguistic analysis, false flag considerations.
- **Santosh Kumar:** Co-author of Technical Analysis, timeline reconstruction, historical patterns. Contributions: TTP comparisons, sophistication, integrated synthesis.

We conducted joint sessions for ATT&CK mapping, unique technique identification, and evolution analysis. Weekly reviews aligned terminology, verified citations, and unified confidence statements.

---

## Directory Structure
```
Threat_Hunters_1_Attribution_Analysis/
├── Attribution_Report.pdf                 # 5–7 pages: executive summary, technical & contextual analysis, attribution assessment
├── Threat_Actor_Comparison_Matrix.xlsx    # APT comparison with scoring and confidence
├── Recommendations_Document.pdf           # Strategic recommendations for attribution & defense
├── Supporting_Evidence/
│   ├── technical_analysis.pdf             # Malware indicators, TTPs, sophistication/resources
│   ├── infrastructure_research.pdf        # C2, domains/IPs, OPSEC, attribution indicators
│   └── geopolitical_context.pdf           # Timing, motives, historical patterns, implications
└── README.md                              # This document
```

### File Descriptions
1. **Attribution_Report.pdf**
   - Content: Executive summary; technical (malware, infra, TTPs); contextual (geopolitics, linguistic, targeting); attribution assessment; challenges (false flags, shared tools); limitations; timeline; alternative hypotheses.
   - Contributors: Imtiyaz (lead, compilation), Yusuf (TTPs), Laiba (malware), Santosh (timeline).

2. **Threat_Actor_Comparison_Matrix.xlsx**
   - Content: Groups (e.g., Sandworm, APT28, APT29, Lazarus, APT40) with capabilities, preferred TTPs, historical targets, infra themes, contradictory evidence, confidence.
   - Features: Scoring formulas, color-coded confidence, ATT&CK references.

3. **Recommendations_Document.pdf**
   - Content: Technical improvements (forensics, ML), international cooperation (NATO, exercises), policy/legal frameworks, defensive measures (ICS segmentation, training).
   - Contributors: Imtiyaz (lead), Santosh (policy), Laiba (defenses), Yusuf (cooperation).

4. **Supporting_Evidence/technical_analysis.pdf**
   - Content: Malware hashes/traits, family research, code reuse, ATT&CK table, sophistication/resources; reproducible steps.
   - Lead: Yusuf; support: Imtiyaz, Laiba, Santosh.

5. **Supporting_Evidence/infrastructure_research.pdf**
   - Content: C2 investigation, domain/WHOIS patterns, hosting/ASN, OPSEC, attribution indicators (IPs, certificates, registrars), timeline.
   -  Lead: Imtiyaz; support: Yusuf, Laiba, Santosh.

6. **Supporting_Evidence/geopolitical_context.pdf**
   - Content: Timing vs events, motives/beneficiaries, historical precedent, diplomatic/economic factors, implications.
   - Lead: Yusuf; support: Imtiyaz, Laiba, Santosh.

---

## Methodology & Frameworks
### Research Process
- Data collection: VirusTotal (hashes), Shodan (IPs), MITRE ATT&CK (TTPs), cross-verified with ESET, Dragos, CISA, RAND, CSIS.
- Analysis tools: Static (IDA Pro, FLOSS), dynamic (Cuckoo Sandbox), network (Wireshark). Reproducible steps favored over proprietary tooling.
- Attribution approach: Diamond Model, Cyber Kill Chain, and ATT&CK mapping. Confidence tiers applied per evidence strength.
- Ethics: Public sources only; facts vs analysis clearly labeled; academic integrity maintained.

### Confidence Level Rubric
- **High:** Strong technical and contextual correlation with multiple independent indicators.
- **Medium:** Partial match with some ambiguity or missing corroboration.
- **Low:** Weak indicators; primarily circumstantial or inconsistent.

### Tools and Frameworks
- MITRE ATT&CK Framework
- Diamond Model of Intrusion Analysis
- Cyber Kill Chain
- Threat intelligence baselining with vendor and government reporting

---

## Work Plan, Responsibilities, and Deadlines
- Attribution_Report.pdf → Lead: Yusuf | Co-author: Laiba (Due: Aug 18)
- Threat_Actor_Comparison_Matrix.xlsx → Lead: Laiba | Support: Santosh (Due: Aug 18)
- Recommendations_Document.pdf → Lead: Imtiyaz | Co-author: Santosh (Due: Aug 18)
- technical_analysis.pdf → Lead: Yusuf | Support: Imtiyaz (Due: Aug 17)
- infrastructure_research.pdf → Lead: Imtiyaz | Support: Yusuf (Due: Aug 17)
- geopolitical_context.pdf → Lead: Yusuf | Support: Laiba (Due: Aug 17)
- README.md → Lead: Santosh | Reviewer: All (Due: Aug 19)

### Review & Quality Control (Aug 18–19)
- Peer reviews: Yusuf → Matrix.xlsx; Laiba → Recommendations.pdf; Imtiyaz → Attribution_Report.pdf; Santosh → Geopolitical_Context.pdf.
- Final QC: Align terminology, verify citations/URLs, unify confidence statements and scoring thresholds.

### Quality Checklist (What “Done” Looks Like)
- Clear separation of evidence vs assessment and explicit confidence level.
- ATT&CK technique IDs included where relevant; tables or concise bullets for indicators.
- All references include working URLs; hashes/IPs cross-verified by at least two sources.
- Reproducible steps documented for any analysis claim.

---

## Navigation & Usage
1. Start with `Attribution_Report.pdf` for the overall narrative and assessment.
2. Use `Threat_Actor_Comparison_Matrix.xlsx` for quick APT comparisons and confidence scoring.
3. Read `Recommendations_Document.pdf` for actionable improvements.
4. Dive into `Supporting_Evidence/` for detailed technical/contextual breakdowns:
   - `technical_analysis.pdf`: Malware and TTPs.
   - `infrastructure_research.pdf`: Network/C2 and OPSEC.
   - `geopolitical_context.pdf`: Motives, timing, implications.

---

## Contribution Guide (Git Workflow)
1. Clone the repository:
   ```bash
   git clone <repo-url>
   ```
2. Create a feature branch:
   ```bash
   git checkout -b <your-task-branch>
   # e.g., git checkout -b yusuf-technical-analysis
   ```
3. Commit your work:
   ```bash
   git add .
   git commit -m "Add technical analysis draft"
   ```
4. Push and open a PR:
   ```bash
   git push origin <your-task-branch>
   ```
5. Request peer review and address feedback prior to merge.

---

## Submission
- Drafts ready: Aug 18
- Peer review complete: Aug 19
- Final submission: Aug 20, 2025
- Packaging: Zip the folder as `Threat_Hunters_1_Attribution_Analysis.zip` for submission.
  ```bash
  cd ..
  zip -r Threat_Hunters_1_Attribution_Analysis.zip Threat_Hunters_1_Attribution_Analysis
  ```

---

## Acknowledgments
Thanks to the assessment coordinator for guidance. All members contributed to discussions, mapping sessions, and peer reviews.

## License
Educational, non-commercial use. For public sharing, this work may be distributed under the Creative Commons Attribution–NonCommercial 4.0 International (CC BY-NC 4.0). If the project remains internal per course policy, treat as internal academic material.

## References (selected)
- MITRE ATT&CK (enterprise matrix)
- CISA advisories on ICS/OT threats
- ESET and Dragos reporting on Ukraine grid intrusions
- RAND and CSIS analytical reports on state-sponsored cyber operations
