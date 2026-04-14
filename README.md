CLEAR LAI Navigation Platform
CLEAR Executive Language Access Certificate Program
Culturally and Linguistically Effective Action for Results
---
Repository Contents
```
/
├── CLEAR_Training_Platform.html            ← 10-Step Executive Training Program (NEW)
├── index.html                              ← LAI Navigation Platform (Tiers 1–3 + Exercises)
├── roi-simulator.html                      ← ROI & Readiness Dashboard
├── data/
│   └── LAI_Q1_2026_Sample_Dataset.xlsx    ← Sample encounter dataset (1,000 LEP encounters)
├── curriculum/
│   └── CLEAR_Module_0_Orientation_DRAFT.docx  ← Module 0 participant document
└── README.md
```
---
Tools Overview
1. CLEAR Executive Training Platform (`CLEAR_Training_Platform.html`)
A 10-step structured executive learning program. Guides participants through the full CLEAR curriculum with embedded evidence, LAI and ROI tool integrations, and document generation at Step 10.
Step	Title	Phase
1	Organization & Baseline	Foundation
2	Pre-Arrival & Triage Access	Evidence
3	Clinical Evaluation & Diagnostic Risk	Evidence
4	Inpatient Reliability & Rework	Evidence
5	Discharge & Comprehension	Evidence
6	Post-Discharge Safety & Risk	Evidence
7	Governance & Execution Variance	Evidence
8	The Full Financial Case	Financial Case
9	Customized Action Plan	Your Plan
10	Board Presentation & Documents	Your Plan
Step 10 generates three downloadable documents:
`CLEAR_CAP_[OrgName].docx` — 8-module CAP · 30-Day Commitment · Governance Structure
`CLEAR_ROI_Summary_[OrgName].xlsx` — All 6 ROI modules · Inputs · System Totals
`CLEAR_BoardPresentation_[OrgName].docx` — 4-component board argument
Tool integration: Each evidence step launches `index.html` (LAI platform) and `roi-simulator.html` (ROI Dashboard) in new tabs. All three files must be in the same directory.
---
2. LAI Navigation Platform (`index.html`)
A 3-tier evidence-based decision support platform.
Tab	Name	Purpose
Tier 1	Self-Assessment	LAI Preparedness Pulse · 10-domain pillar scores
Tier 2	Hypothesis Builder	Structured hypothesis formation before evidence review
Tier 3	Performance Review	Statistical testing against encounter data
Exercises	Module Simulations	18 hands-on statistical exercises — 3 per curriculum module
Financial Stewardship domain KPIs (updated):
KPI 1: % of language access cost exposure streams (readmission penalties, LOS differential, malpractice risk, VBP impact) actively tracked, quantified & reported to financial leadership
KPI 2: % of LEP inpatient encounters with LOS outcomes tracked by preferred language & benchmarked vs. English-proficient cohorts
---
3. ROI & Readiness Dashboard (`roi-simulator.html`)
Financial impact modeling across six domains.
Module	ROI Domain	Curriculum Alignment
ED Language Access & Stroke	Revenue preservation from timely interpreter access	Module 1 / Step 2
Engagement & LOS Reduction	Length-of-stay savings from communication best practices	Module 3 / Step 4
Teach-Back (Dual)	Readmission avoidance with S-curve automation	Module 4 / Step 5
Malpractice Cost-Avoidance	Two-track: damage + defense cost avoidance	Module 5 / Step 6
State Reimbursement	Medicaid interpreter billing offset	Modules 5–6 / Step 6
Value-Based Care (VBP)	Medicare quality withhold recapture	Module 6 / Step 7
---
Deployment: GitHub Pages
Quick Setup
Fork or clone this repository
Go to Settings → Pages
Set source to `main` branch, root folder `/`
Click Save
Your tools will be live at:
```
https://[your-org].github.io/[repo-name]/CLEAR_Training_Platform.html  → Training Platform
https://[your-org].github.io/[repo-name]/                               → LAI Platform
https://[your-org].github.io/[repo-name]/roi-simulator.html             → ROI Dashboard
```
Important: All three HTML files must be in the same directory so the training platform's tool-launch buttons resolve correctly.
---
Articulate 360 Embedding
Rise (recommended)
Add a Web Object content block
Paste the GitHub Pages URL for `CLEAR_Training_Platform.html`
Set height to `700px` minimum; enable scrolling
Recommended flow per module (standalone LAI use)
```
LAI Platform (Tier 2 hypothesis)
  → LAI Platform (Tier 3 statistical results)
  → ROI Dashboard (financial translation)
  → Reflection / CAP entry
```
---
Sample Dataset
`data/LAI_Q1_2026_Sample_Dataset.xlsx` — 1,000 simulated LEP encounters, 85 variables.
Upload instructions (LAI Platform):
Open `index.html`
Navigate to Tier 3 → Performance Review
Click the upload zone and select the dataset file
---
Module-by-Module Integration Map
Module	Training Step	LAI Exercises	ROI Module	Note
0 · Orientation	Step 1	Tier 1 Self-Assessment	Observe dashboard	—
1 · Pre-Arrival & Triage	Step 2	Module 1 (Ex 1.1–1.3)	ED Language Access & Stroke	—
2 · H&P & Diagnostic	Step 3	Module 2 (Ex 2.1–2.3)	Workflow Simulation Lab	—
3 · Inpatient Rounding	Step 4	Module 3 (Ex 3.1–3.3)	Engagement & LOS Reduction	—
4 · Discharge	Step 5	Module 4 (Ex 4.1–4.3)	Teach-Back (Dual)	—
5 · Post-Discharge / Safety	Step 6	LAI Module 6 (Ex 6.1–6.3)	Malpractice + State Reimbursement	⚠ Uses Exercise Set 6
6 · Governance	Step 7	LAI Module 5 (Ex 5.1–5.3)	VBP	⚠ Uses Exercise Set 5
7 · CAP Capstone	Steps 9–10	—	All modules	Document generation
> **Exercise Set Note:** Curriculum Module 5 (Post-Discharge/Safety) uses LAI Exercise Set 6, and curriculum Module 6 (Governance) uses LAI Exercise Set 5. The training platform directs learners to the correct set automatically.
---
Technical Notes
No build pipeline required. All three HTML files are fully self-contained.
No server required. GitHub Pages serves static files.
No login or authentication. Publicly accessible.
Browser compatibility. Chrome 90+, Firefox 88+, Safari 14+, Edge 90+.
File sizes: `CLEAR_Training_Platform.html` ~131KB · `index.html` ~410KB · `roi-simulator.html` ~183KB
---
License & Use
This platform and curriculum were developed for the CLEAR Executive Language Access Certificate Program. All content is proprietary. Intended for licensed program participants only.
