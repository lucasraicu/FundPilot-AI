# Graph Report - FundProof  (2026-11-15)

## Corpus Check
- 101 files · ~59,074 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 18 file(s) not represented in the graph (top: .csv 7, (none) 3, .css 3)

## Summary
- 586 nodes · 1204 edges · 38 communities (25 shown, 13 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 65 edges (avg confidence: 0.86)
- Token cost: 369,110 input · 0 output

## Community Hubs (Navigation)
- Analysis UI Components
- Allocation Splits & Eval
- Legacy Demo Grants A/B
- Claude Rule Extraction
- Analyze & Dataset API
- Dataset Loading & Parsing
- Streamlit Frontend
- Allocation Prompt Rules
- Dev Dependencies
- Evidence Drawer & Upload
- Research Impact Page
- TypeScript Config
- Grant Clauses & Brightpath
- Federal Subaward FLS
- Foundation Grant HFF
- Team Rules & Murmur
- Runtime Dependencies
- Shared Contract & Mock
- Core Design Principles
- Pipeline Steps & Citations
- ESLint Config
- Demo Modes & Fallbacks
- Savings Model Research
- Legacy Demo Answer Key
- npm Scripts
- Issue & PR Templates
- Unrestricted Fund Staff
- Alcohol Cost Rule
- Entertainment Cost Rule
- Fundraising Cost Rule
- Node Types
- PostCSS Config
- Next/Vercel Logos
- File Icon
- Globe Icon
- Window Icon

## God Nodes (most connected - your core abstractions)
1. `loadDataset()` - 21 edges
2. `compilerOptions` - 16 edges
3. `FundProofWorkspace()` - 15 edges
4. `AnalysisResult` - 15 edges
5. `normalizeUpload()` - 14 edges
6. `analyzeUploads()` - 13 edges
7. `UploadError` - 13 edges
8. `inspectDocument()` - 12 edges
9. `Dataset` - 12 edges
10. `Grant Agreement HFF-26-118: After-School Tutoring Program` - 12 edges

## Surprising Connections (you probably didn't know these)
- `Proposed Backend Contract (POST /analyze, funds/transactions)` --semantically_similar_to--> `AnalysisResult`  [AMBIGUOUS] [semantically similar]
  frontend/README.md → CLAUDE.md
- `Grant A: Payroll requires dated activity/time records` --semantically_similar_to--> `Curated Federal Subset: 2 CFR 200.403, 200.405, 200.430(g)`  [INFERRED] [semantically similar]
  demo/Grant_A_Digital_Skills.pdf → docs/PLAN.md
- `Expected Review Cases T001-T009 (legacy kit answer key)` --semantically_similar_to--> `data/expected.json answer key`  [INFERRED] [semantically similar]
  demo/EXPECTED_TEST_CASES_DO_NOT_UPLOAD.txt → README.md
- `Legacy demo/ bundle unsupported` --references--> `FundProof Synthetic Hackathon Demo Kit (legacy)`  [INFERRED]
  data/examples/README.md → demo/README_START_HERE.txt
- `INV-T009 Training Specialist LLC $480 (T009, no payment evidence)` --conceptually_related_to--> `Status Semantics (Supported / Needs Evidence / Conflict / Not Eligible)`  [INFERRED]
  demo/Sample_Receipts_and_Invoices.pdf → docs/PLAN.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **FundProof analysis pipeline (extract rules, propose, compute, verify)** — claude_extractrules, claude_proposeallocations, claude_computesplits, claude_verifycitations, claude_api_analyze [EXTRACTED 1.00]
- **Three-state demo evidence flow** — docs_demo_held_evidence_story, docs_demo_maria_lopez_case, docs_demo_brightpath_case, data_inputs_brightpath_scope_of_work_scope_of_work, data_claude_runs_readme_demo_states [EXTRACTED 1.00]
- **Federal subaward clauses driving demo decisions** — data_source_grant_fed_agreement_alcohol_clause, data_source_grant_fed_agreement_budget_estimates_clause, data_source_grant_fed_agreement_contracted_services_clause, docs_demo_luna_bistro_case, docs_demo_maria_lopez_case, docs_demo_brightpath_case [EXTRACTED 1.00]
- **Proposal prompt iterations: initial, timesheet fix, scope of work** — data_claude_runs_prompts_2_proposals_initial_proposals_prompt, data_claude_runs_prompts_3_proposals_after_fix_proposals_prompt, data_claude_runs_prompts_4_proposals_scope_of_work_proposals_prompt [INFERRED 0.85]
- **Contractor charge evidence: T-003 against FED-R10/FDN-R4 resolved by scope of work** — data_claude_runs_prompts_2_proposals_initial_t_003_brightpath, data_claude_runs_prompts_2_proposals_initial_fed_r10, data_claude_runs_prompts_2_proposals_initial_fdn_r4, data_claude_runs_prompts_4_proposals_scope_of_work_brightpath_scope_of_work [INFERRED 0.85]
- **Payroll timesheet consistency check for E-01** — data_claude_runs_prompts_2_proposals_initial_pay_e_01, data_claude_runs_prompts_2_proposals_initial_e_01_timesheet_missing_fdn, data_claude_runs_prompts_3_proposals_after_fix_e_01_corrected_timesheet, data_claude_runs_prompts_2_proposals_initial_payroll_time_records_rule, data_claude_runs_prompts_2_proposals_initial_fed_r8 [INFERRED 0.85]
- **Fail-closed evidence integrity (validation, verified badge, statuses, cents in code)** — docs_plan_deterministic_validation, docs_plan_source_verified_badge, docs_plan_status_semantics, docs_plan_shared_types_contract [INFERRED 0.85]
- **Demo receipts exercising grant eligibility rules** — demo_sample_receipts_and_invoices_r_t004, demo_sample_receipts_and_invoices_r_t005, demo_grant_a_digital_skills_food_exclusion_rule, demo_grant_a_digital_skills_equipment_preapproval_rule, demo_grant_b_outreach_capital_equipment_exclusion [INFERRED 0.85]
- **Lane coordination via Murmur (message types, lead checkpoints, lanes)** — docs_murmur_message_types, docs_murmur_lead_agent_role, docs_murmur_checkpoint_schedule, docs_plan_work_lanes [INFERRED 0.85]
- **Allowable uses of grant funds (Section 2)** — data_inputs_grant_fdn_agreement_rule_2_1, data_inputs_grant_fdn_agreement_rule_2_2, data_inputs_grant_fdn_agreement_rule_2_3 [EXTRACTED 1.00]
- **Restrictions on grant funds (Section 3)** — data_inputs_grant_fdn_agreement_rule_3_1, data_inputs_grant_fdn_agreement_rule_3_2, data_inputs_grant_fdn_agreement_rule_3_3 [EXTRACTED 1.00]
- **Section 3 unallowable cost rules** — data_inputs_grant_fed_agreement_rule_3_1_alcohol_unallowable, data_inputs_grant_fed_agreement_rule_3_2_entertainment_unallowable, data_inputs_grant_fed_agreement_rule_3_3_fundraising_unallowable, data_inputs_grant_fed_agreement_rule_3_4_other_programs_excluded, data_inputs_grant_fed_agreement_rule_3_5_general_operating_excluded [EXTRACTED 1.00]
- **Section 4 documentation requirements** — data_inputs_grant_fed_agreement_rule_4_1_personnel_records, data_inputs_grant_fed_agreement_rule_4_2_budget_estimates_insufficient, data_inputs_grant_fed_agreement_rule_4_3_contracted_services_agreement [EXTRACTED 1.00]
- **create-next-app Default Starter Icon Set (file, globe, window)** — public_file_file_icon, public_globe_globe_icon, public_window_window_icon [INFERRED 0.85]

## Communities (38 total, 13 thin omitted)

### Community 0 - "Analysis UI Components"
Cohesion: 0.08
Nodes (55): AnalysisCharts(), money(), CsvPreview(), DemoAnalysisVisualization(), stages, DemoCorrection(), choose(), CsvPreviewData (+47 more)

### Community 1 - "Allocation Splits & Eval"
Cohesion: 0.10
Nodes (42): proposeAllocations(), apportion(), percentsFromTimesheets(), splitByPercent(), cents(), evaluateAnalysis(), ExpectedItems, isMoney() (+34 more)

### Community 2 - "Legacy Demo Grants A/B"
Cohesion: 0.05
Nodes (44): Grant A Approved Budget (materials $4k, staff $8k, transport $2k, admin $1k), Grant A: Equipment over $500 requires written prior approval, Grant A: Food, entertainment, personal purchases excluded, Grant Agreement A: Digital Skills (DSG-2026-041, Oakridge Community Trust, $15,000), Grant A: Payroll requires dated activity/time records, Grant B Approved Budget (events $3.5k, staff $5k, transport $1.5k, printing $2k), Grant B: Capital equipment above $300 excluded, Grant Agreement B: Neighborhood Outreach (NOG-2026-022, Cedar Foundation, $12,000) (+36 more)

### Community 3 - "Claude Rule Extraction"
Cohesion: 0.11
Nodes (32): callStructured(), getClient(), MODEL, pdfBlock(), UserContent, extractRulesForFund(), RULES_SYSTEM, RuleSchema (+24 more)

### Community 4 - "Analyze & Dataset API"
Cohesion: 0.12
Nodes (28): accountProblem(), fromCache(), maxDuration, pause(), POST(), runtime, Scenario, scenarioFor() (+20 more)

### Community 5 - "Dataset Loading & Parsing"
Cohesion: 0.11
Nodes (24): MAX_FILE_BYTES, csv(), dollars(), field(), FUND_TYPE, fundCode(), hours(), isFundCode() (+16 more)

### Community 6 - "Streamlit Frontend"
Cohesion: 0.09
Nodes (11): analyze(), is_excluded_document(), validate(), dashboard_chart(), table(), sample_data(), demo_data.py synthetic fixtures, Proposed Backend Contract (POST /analyze, funds/transactions) (+3 more)

### Community 7 - "Allocation Prompt Rules"
Cohesion: 0.12
Nodes (22): 2 CFR Part 200 (Uniform Guidance), E-01 Timesheet Without Tutoring Hours (120 FED / 40 UNRESTRICTED), FDN-R4 Consultants Require Prior Written Approval, Foundation Grant Rules FDN-R1..R8, FED-R10 Written Agreement For Contracted Services, FED-R8 Personnel Records Requirement (2 CFR 200.430(i)), Federal Grant Rules FED-R1..R12, GRANT-FDN Hartwell Family Foundation Tutoring Grant (HFF-26-118) (+14 more)

### Community 8 - "Dev Dependencies"
Cohesion: 0.12
Nodes (22): devDependencies, eslint@^9, eslint-config-next@15.5.4, tailwindcss@^4, @tailwindcss/postcss@^4, tsx@^4.23.15, @types/papaparse@^5.5.2, @types/react@^19 (+14 more)

### Community 9 - "Evidence Drawer & Upload"
Cohesion: 0.15
Nodes (17): EvidenceDrawer(), money(), statuses, aliases, date(), derivedId(), grantFund(), headerMap() (+9 more)

### Community 10 - "Research Impact Page"
Cohesion: 0.14
Nodes (11): documentHtml, ResearchImpact(), researchImpactHtml, ResearchImpactNavigation(), geistMono, geistSans, metadata, RootLayout() (+3 more)

### Community 11 - "TypeScript Config"
Cohesion: 0.11
Nodes (18): compilerOptions, allowJs, esModuleInterop, incremental, isolatedModules, jsx, lib, module (+10 more)

### Community 12 - "Grant Clauses & Brightpath"
Cohesion: 0.15
Nodes (17): Brightpath Consulting LLC, Deliverables 2.1-2.3 (assessment rubric, training, baseline report), Brightpath Scope of Work (Contract EYL-2026-C07), HFF Budget ($45,000; $22,500 remaining), Clause 3.1: no consultants without prior written approval, Grant Agreement HFF-26-118 (Hartwell Family Foundation, GRANT-FDN), Clause 4.1: maintain staff time records, 2 CFR 200 (Uniform Guidance) (+9 more)

### Community 13 - "Federal Subaward FLS"
Cohesion: 0.12
Nodes (9): Subaward Agreement: Federal Literacy Program (FLS-2026-0412), 2 CFR 200.405 (allocable costs), 2 CFR 200.430(i) (personnel documentation standards), Approved Budget ($96,000 total; $48,200 remaining as of Oct 1 2026), Instructional materials and software budget ($24,000 approved, $11,800 remaining), Personnel and fringe budget ($72,000 approved, $36,400 remaining), Eastbay Youth Literacy (subrecipient), Federal Literacy Program (+1 more)

### Community 14 - "Foundation Grant HFF"
Cohesion: 0.19
Nodes (7): After-School Tutoring Program, Grant Agreement HFF-26-118: After-School Tutoring Program, Grant Budget (total $45,000, $22,500 remaining as of Oct 1 2026), Budget: Tutoring program staff ($33,000 approved, $16,500 remaining as of Oct 1 2026), Budget: Books, supplies and student snacks ($12,000 approved, $6,000 remaining), Eastbay Youth Literacy (Grantee), Hartwell Family Foundation (Grantor)

### Community 15 - "Team Rules & Murmur"
Cohesion: 0.24
Nodes (7): Murmur, Repository Instructions (AGENTS.md), npm run eval (live pipeline vs data/expected.json), FundProof Team Rules (CLAUDE.md), Murmur Message Types ([CONTRACT],[LANDED],[ASK],[BLOCKED],[EVAL],[REVIEW],[CHECKPOINT],[FREEZE]), data/expected.json answer key, FundProof README

### Community 16 - "Runtime Dependencies"
Cohesion: 0.18
Nodes (11): dependencies, @anthropic-ai/sdk@^1.8.0, papaparse@^5.7.1, postal-mime@^4.2.1, react-dom@19.1.0, read-excel-file@^9.3.17, unpdf@^1.9.1, @anthropic-ai/sdk (+3 more)

### Community 17 - "Shared Contract & Mock"
Cohesion: 0.22
Nodes (8): AnalysisResult, POST /api/analyze, Shared Contract lib/types.ts, POST/GET /api/dataset, buildMockAnalysis, Mock Upload Examples, mockAnalysis field, Upload limits (20 files, 10MB/file, 40MB total)

### Community 18 - "Core Design Principles"
Cohesion: 0.20
Nodes (8): computeSplits (lib/data/computeSplits.ts), buildResult (lib/pipeline.ts), Clause 4.2: budget estimates do not qualify as support, Maria Lopez payroll case ($7,440 split 96/32/32 hours), Lane Issues (#5 UI, #6 AI, #7 DATA), Hackathon Milestones (setup 1:30, freeze 4:15, demo 4:30), Project Overview (TASKS.md), Stack: Next.js 15 + TypeScript + Tailwind + @anthropic-ai/sdk + zod

### Community 19 - "Pipeline Steps & Citations"
Cohesion: 0.33
Nodes (8): extractRules (lib/ai/extractRules.ts), FundProof, proposeAllocations (lib/ai/proposeAllocations.ts), verifyCitations (lib/data/verifyCitations.ts), Rule JSON Schema (kind/summary/page/quote), Rule Extraction Prompt (GRANT-FDN), Rule JSON Schema (kind/summary/page/quote), Rule Extraction Prompt (GRANT-FED)

### Community 20 - "ESLint Config"
Cohesion: 0.22
Nodes (6): compat, __dirname, eslintConfig, __filename, @eslint/eslintrc@^3, @eslint/eslintrc

### Community 21 - "Demo Modes & Fallbacks"
Cohesion: 0.36
Nodes (8): FUNDPROOF_MOCK env flag, Mock Fixtures (lib/fixtures/*.json), Three demo states (initial, after-fix, scope-of-work), FUNDPROOF_MOCK=cache mode, Recorded Claude Runs, Demo Script (under 2 minutes), Demo fallbacks (cache -> mock fixtures), $10,940 -> $3,500 -> $0 held story

### Community 22 - "Savings Model Research"
Cohesion: 0.32
Nodes (8): Demo totals: 13 costs, $27,752.28, Illustrative savings model (6 h/wk, $35/h, 25-75%), Impact Assumptions (impact-assumptions.json), BLS occupation wage benchmarks (May 2025), Community Brands / GiveSmart 2024 Nonprofit Research Study, FundPilot-AI Demo Companion Page, Annual hours/labor value savings chart (25/50/75%), Loaded wage calc (BLS wage / (1 - benefits share))

### Community 23 - "Legacy Demo Answer Key"
Cohesion: 0.29
Nodes (6): Expected Review Cases T001-T009 (legacy kit answer key), T003 payroll split by time records (no invented 50/50), FundProof Synthetic Hackathon Demo Kit (legacy), evidence_register.csv (assertions, not proof), Grant A Digital Skills, Grant B Outreach

### Community 24 - "npm Scripts"
Cohesion: 0.29
Nodes (7): scripts, build, dev, eval, lint, start, typecheck

## Ambiguous Edges - Review These
- `AnalysisResult` → `Proposed Backend Contract (POST /analyze, funds/transactions)`  [AMBIGUOUS]
  frontend/README.md · relation: semantically_similar_to

## Knowledge Gaps
- **50 isolated node(s):** `Task Issue Template`, `Murmur Message Types ([CONTRACT],[LANDED],[ASK],[BLOCKED],[EVAL],[REVIEW],[CHECKPOINT],[FREEZE])`, `Hackathon Milestones (setup 1:30, freeze 4:15, demo 4:30)`, `Stack: Next.js 15 + TypeScript + Tailwind + @anthropic-ai/sdk + zod`, `Lane Issues (#5 UI, #6 AI, #7 DATA)` (+45 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 167 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **13 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `data/expected.json answer key` connect `Team Rules & Murmur` to `Claude Rule Extraction`, `Legacy Demo Answer Key`?**
  _High betweenness centrality (0.147) - this node is a cross-community bridge._
- **What connects `Task Issue Template`, `Murmur Message Types ([CONTRACT],[LANDED],[ASK],[BLOCKED],[EVAL],[REVIEW],[CHECKPOINT],[FREEZE])`, `Hackathon Milestones (setup 1:30, freeze 4:15, demo 4:30)` to the rest of the system?**
  _50 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Analysis UI Components` be split into smaller, more focused modules?**
  _Cohesion score 0.07945566286215978 - nodes in this community are weakly interconnected._
- **Why does `Expected Review Cases T001-T009 (legacy kit answer key)` connect `Legacy Demo Answer Key` to `Team Rules & Murmur`?**
  _High betweenness centrality (0.087) - this node is a cross-community bridge._
- **Should `Allocation Splits & Eval` be split into smaller, more focused modules?**
  _Cohesion score 0.10168350168350168 - nodes in this community are weakly interconnected._
- **Why does `FundProof Streamlit Frontend` connect `Streamlit Frontend` to `Legacy Demo Answer Key`?**
  _High betweenness centrality (0.070) - this node is a cross-community bridge._

### Low-confidence Hints
_AMBIGUOUS edges — the extractor was unsure. Verify before acting on these._

- **What is the exact relationship between `AnalysisResult` and `Proposed Backend Contract (POST /analyze, funds/transactions)`?**
  _Edge tagged AMBIGUOUS (relation: semantically_similar_to) - confidence is low._