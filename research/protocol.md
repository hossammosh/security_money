# Research protocol proposal — not a completed paper

## Working title
Evidence-Grounded AI Assistance for Reproducible Mobile-App Bug Reports: A Controlled Pilot Study

Status: proposed study; novelty not established; data, sample size, models, venue, and budget not finalized. No results exist.

## Motivation and boundary
Connect practical QA skills with deep-learning research without repurposing confidential paid-testing data. Functional bug-report research is software-engineering research; it should not be labeled a cybersecurity evaluation unless genuine security outcomes are separately designed and tested.

## Prior art inspected
1. ReCoDe / Mobile App Crowdsourced Test Report Consistency Detection via Deep Image-and-Text Fusion Understanding. Abstract and version history inspected: https://arxiv.org/abs/2108.07401 (v3, 2023); related journal DOI https://doi.org/10.1109/TSE.2023.3285787 . Work already studies text/screenshot consistency with deep learning. Full paper, dataset license, and reuse rights need review before reuse.
2. Large Language Models for Mobile GUI Text Input Generation: An Empirical Study. Abstract and version history inspected: https://arxiv.org/abs/2404.08948 (v4, 2026). Work already studies LLM-assisted Android testing, context representations, feedback, and human assistance. Full paper and artifacts need review.

These papers establish related work, not an absence of competing work. 'Using AI for app testing' is not, by itself, a defensible novelty claim. Conduct a broader current literature review before fixing the contribution.

## Candidate research questions
RQ1: Does evidence-constrained AI assistance improve independent reproduction success compared with a structured non-AI report template?
RQ2: How often does unconstrained assistance add unsupported steps or observations, compared with evidence-constrained assistance?
RQ3: What are the time, inference cost, and quality trade-offs for local versus hosted assistance on publication-cleared data?
RQ3 is optional; keep scope feasible and do not conflate local execution with a complete privacy guarantee.

## Data and experimental environment
- Start with one or two open-source Android apps run locally in an emulator/device, with explicit license and asset checks.
- Prefer known reproducible bugs or clearly labeled seeded bugs. Record app version, commit, OS, device/emulator, and reset procedure.
- Use only recordings, logs, and screenshots made in the research environment with synthetic accounts and data.
- Public availability alone does not grant redistribution rights. Review data licenses and privacy, including third-party issues/screenshots.
- No paid client reports, binaries, fees, platform invitations, or customer data by default.
- Potentially real vulnerabilities in open-source targets require responsible disclosure before release.

## Candidate conditions
A: structured report template, no AI.
B: generic AI report assistance using the same permitted evidence.
C: evidence-grounded assistance requiring explicit evidence references for each factual claim and an 'unknown' response when evidence is absent.

Keep evidence, time budget, and task difficulty comparable. Fix and record model versions, prompts, decoding settings, and tool access. Repeat stochastic runs where justified. Clearly distinguish seeded from naturally occurring bugs.

## Pilot then confirmatory evaluation
Begin with a small feasibility pilot. Select final sample size from pilot variance, a practically meaningful effect, and an appropriate power/precision analysis; do not claim that a convenient small sample establishes broad effectiveness.

Use independent raters/testers where possible, blind to report condition, randomized/counterbalanced ordering, reset environments, and controls for learning/carryover. If using multiple human participants or their behavior/data, obtain informed consent and appropriate institutional ethics review or documented determination before collection. A single-author self-study can be a pilot but does not support population-level claims about novice testers.

## Measurements
Primary: independent reproduction success under a fixed protocol.
Secondary: completion time including verification/correction; report completeness under a predefined rubric; unsupported factual claims; model cost and latency; reviewer agreement; robustness across apps/bug classes.

Predefine the unit of analysis (bug/app/participant), handle clustering and repeated measures, report effect sizes and confidence intervals, and document exclusions/missing data. Do not treat repeated prompts on one bug as independent real-world bugs.

## Bias and reproducibility safeguards
Split by app/bug family where suitable; avoid tuning on evaluation cases; report possible training-data contamination; do not make an LLM judge the sole ground truth. Preserve negative results. Release only licensed, reviewed artifacts and allowed data.

## Publication route
Select a legitimate software-testing/software-engineering venue after reviewing fit, scope, novelty, author instructions, ethics and AI-use requirements. A preprint is not peer-reviewed acceptance. No acceptance, citation, deadline, or publication fee is assumed. AI may assist drafting, but humans must verify every citation, claim, experiment, and result. Never fabricate participants, measurements, or findings.
