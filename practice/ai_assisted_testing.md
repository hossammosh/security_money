# AI-assisted testing: practice and work safely

## Principle
AI assists the tester; it does not supply evidence. You must observe and reproduce findings. Do not use fabricated screenshots, invented steps, or unsupported severity claims. Functional QA authorization is not penetration-testing authorization.

## Roles
AI: explain concepts, generate generic edge-case checklists for synthetic workflows, suggest a report structure, and review permitted practice examples.
Tester: read scope/terms, execute authorized checks, verify observations, rule out expected behavior, gather allowed evidence, and submit only accurate findings.

## Client information gate
Default: do NOT paste client names, URLs, private app screenshots/builds, reports, test cases, logs, or instructions into an external AI tool. Obtain explicit applicable permission first. Sanitizing or a local model does not override contractual restrictions. Do not scrape a platform, use bots, or scan targets without authorization.

## Safe practice prompt 1 — generic checklist
"I am practicing functional QA on a demo login workflow that I own or am authorized to test. Create a concise manual checklist for valid inputs, invalid inputs, required fields, error messages, keyboard navigation, and basic layout behavior. Do not suggest attacks, scanning, real payment transactions, or out-of-scope actions. Treat every case as a proposal, not an observed result."

## Safe practice prompt 2 — structure, not invented evidence
"Using only the following synthetic practice observations, organize a bug report into title, environment, preconditions, steps, expected result, actual result, reproducibility and evidence. Mark missing details as unknown. Do not invent reproduction steps, severity, screenshots, test execution or device information."

## Safe practice prompt 3 — review
"Review this publication-cleared practice report for ambiguity and missing evidence. List questions I should resolve by manual testing. Do not decide that a bug exists without evidence, and do not add new factual claims."

## Report template
- Title:
- Environment (app version, OS/device/browser):
- Preconditions and synthetic account state:
- Exact reproduction steps:
- Expected behavior and its basis:
- Actual observed behavior:
- Reproduction frequency:
- Allowed evidence:
- Limitations/unknowns:

Do not fill unknown sections with guesses. Use the project's severity rules; a typo is not automatically a security issue. Publish only own practice material with appropriate rights.
