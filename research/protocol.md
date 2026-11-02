> INACTIVE / OPTIONAL: The current priority is AI-assisted practice and remote testing income. Research is not mandatory. This unexecuted proposal is retained only as reference.

# Deep-learning research protocol proposal — no results yet

Updated 2026-11-02 following the explicit requirement that deep-learning research is essential and must proceed alongside field work.

## Working title
Cross-Application Generalization and Uncertainty in Multimodal Deep Learning for Duplicate Mobile-App Bug Report Retrieval

This is a candidate topic, not an approved final paper title or established novel contribution. The previous generic AI-report-assistance proposal is superseded. Do not interpret this revision as evidence that experiments have been conducted.

## Mandatory objective
Do paid remote testing and substantive deep-learning research concurrently. A prompt wrapper or use of Genspark for report writing alone is not the research deliverable. This candidate study includes model implementation/adaptation, a train/validation/test protocol, non-neural and neural baselines, ablations, and an explicit evaluation of limitations. Training a model from scratch is not required. Other rigorous deep-learning research designs remain possible.

## Candidate practical problem
Given a new mobile-app bug report and its permitted screenshot(s), retrieve earlier reports describing the same underlying bug, and flag uncertain matches for human review. This is a prototype research task, not a platform integration or a promise of higher income. Never query or upload a platform's confidential report database or automate platform work without permission.

Duplicate retrieval can be studied using a legally obtained research corpus. Confirming impact on paid-platform acceptance or income would require a separately authorized study and cannot be inferred from offline accuracy.

## Prior art and novelty gate
Previously inspected abstract sources:
- Mobile App Crowdsourced Test Report Consistency Detection via Deep Image-and-Text Fusion Understanding: https://arxiv.org/abs/2108.07401
- Large Language Models for Mobile GUI Text Input Generation: An Empirical Study: https://arxiv.org/abs/2404.08948

These are related examples, not an exhaustive review or a verified gap in duplicate retrieval. Before choosing the final task, review existing duplicate-bug retrieval, multimodal report models, cross-project evaluation, calibration, and selective prediction. Read full papers and verify all citations. Do not claim that combining text and images is novel. Proceed only if an original or meaningful replication/benchmark contribution is justified for the intended venue.

## Proposed architecture — adjustable after feasibility review
- Text branch: pretrained transformer encoding the report description and reproduction steps.
- Image branch: pretrained visual encoder for screenshots.
- Baseline fusion: normalized embedding concatenation or a small learned fusion layer.
- Candidate learned approach: parameter-efficient adaptation/contrastive training using duplicate and nonduplicate report pairs with hard negatives.
- Similarity ranking followed by a validation-set-calibrated acceptance/abstention threshold.

Neural embeddings, multimodal fusion, contrastive learning, and calibration are standard ingredients. Their use alone is not a novelty claim. Inspect screenshots for irrelevant app-identity shortcuts; align branches carefully and record all model/data licenses.

## Research questions
RQ1: Does the adapted multimodal approach outperform lexical and frozen-encoder baselines on unseen applications?
RQ2: How do image/text ablations, hard negatives, and uncertainty thresholds change retrieval quality and false-match rates?
RQ3: What is the quality/latency/compute trade-off on the actual available hardware?

## Baselines and ablations
- TF-IDF or BM25 text retrieval (non-neural).
- Frozen text-encoder retrieval.
- Adapted text-only retrieval.
- Frozen text+image embeddings with simple fusion.
- Adapted text+image approach.
- Matched-budget ablations for image branch, adaptation, hard negatives, and abstention.

Use fair hyperparameter budgets and the same permitted evidence. Do not add complexity unless a simpler model establishes a useful baseline.

## Dataset and ground truth
Select a corpus only after verifying provenance, task fit, license, redistribution rights, privacy, sufficient duplicate labels, and group/app identifiers. A public issue is not automatically a licensed dataset. No suitable corpus is assumed to exist yet.

Fallback: create a clearly labeled pilot on owned/licensed apps with controlled known/seeded bugs, synthetic accounts, screenshots, and independently authored report variants. Disclose that seeded/constructed variants may be unlike real reports. Do not use generated paraphrases as a substitute for independent natural bug evidence or treat many paraphrases of one bug as many independent bugs.

No paid client reports, app builds, customer screenshots, fee data, or internal bug databases. Written permission and applicable privacy/ethics review are required before any exception. Participants and annotators require appropriate consent and ethics determination before collection.

## Evaluation safeguards
Split by application and underlying bug before generating pairs/variants. Never distribute screenshots, duplicates, near-duplicate reports, or variants of the same bug across training and test sets. Keep test apps untouched during tuning. Examine potential pretrained-model contamination and report limits. If there are too few independent apps/bugs, restrict conclusions to a pilot.

Report Recall@k, MRR, and task-appropriate precision/recall for duplicate decisions; false-match rate and risk-coverage for abstention; latency, memory, inference/training cost, and repeated-seed variability. Specify labels, candidate-pool size, negative sampling, and deployment prevalence. Use calibrated probabilities only when a probability model and calibration evaluation support them; raw similarity is not probability.

Use independent human/known-bug ground truth, not only LLM judgments. Report confidence intervals with clustering by independent app/bug as appropriate, effect sizes, failure cases, and negative results. Select sample size from pilot feasibility and precision/power needs rather than convenient report counts.

## Field connection without data leakage
During authorized testing, learn scope reading, reproducibility, device behavior, and report clarity. Use only general transferable skills and permitted public information to shape the research. Re-create safe examples independently. Do not recreate confidential proprietary bugs merely to evade NDA restrictions.

Model use on paid assignments is a separate permission gate. Offline research results alone do not authorize AI use, scraping, automation, or third-party data transfer.

## Publication and reproducibility
Prepare a manuscript only after a defensible study. Release rights-cleared code, configurations, split manifests, model metadata, seeds, and artifacts. Human authors remain accountable; disclose AI assistance according to venue rules. Identify a legitimate testing/software-engineering venue after reviewing contribution fit. Research here is software testing, not validated cybersecurity detection. No earnings, results, deadlines, acceptance, or novelty are promised.
