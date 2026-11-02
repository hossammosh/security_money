# Desktop bug reproduction: beginner guide

Sources reviewed 2026-11-02. Desktop only: the user's critical phone must not be used for testing. These are public learning notes, not client evidence or completed paid work.

## Meaning
A reproduction repeats an existing reporter's steps and checks whether the same bug occurs. Positive: the same bug happens. Negative: after following the same steps, the function works correctly. A different bug, blocked access, a missing precondition or the wrong environment is not proof of a valid negative reproduction.

## Workflow
1. Finish onboarding and work only on available authorized tasks.
2. Read scope, original report, preconditions, test data, environment and task/session instructions. Choose only supported computer tasks; Firefox is not automatically permitted in every task.
3. Follow all original steps. Do not make purchases, enter real payment details, scan, or attack systems unless explicitly authorized and consciously accepted.
4. Observe whether the original bug occurs. If prerequisites cannot be met, do not guess or misclassify the result.
5. Record evidence using the task's requirements. Test IO's rejection guide specifies a screencast not longer than 15 seconds, playable MP4, the triggering action and result visible, browser URL bar and identifiable date visible. For crash bugs the required crash log is needed as well. Do not speed up playback to fit the duration.
6. The full attempt still follows the original steps. Keep the evidence focused on the relevant final navigation/action/result; do not omit required setup from execution just to shorten video. If the required evidence cannot fit, consult the current instructions/team leader rather than editing misleadingly.
7. In the reproduction form choose whether the bug reproduces, select the actual environment, attach the correct screencast, and click Create reproduction. Perform only one platform task at a time as instructed.
8. Review feedback; no acceptance or payment is guaranteed. If a different bug occurs, follow scope and new-report/duplicate rules, not a false negative reproduction.

## Synthetic example — not a real bug report
Original report: search for a specified in-stock item; results unexpectedly show no products.
Same permitted setup + same empty result => positive.
Same permitted setup + correct products returned => negative.
Cannot access the page or a different failure occurs => insufficient basis for that negative result; clarify the task.

## Privacy and AI
Use a separate test browser profile without personal logins/bookmarks. It is not a malware sandbox. Keep customer evidence on authorized channels; do not upload client screenshots, recordings, private URLs, credentials or reports to public GitHub or external AI without applicable permission. Never fabricate observations or use AI-generated evidence.

## Sources
- Definitions and rules: https://academy.test.io/en/articles/2541944-bug-reproductions
- Concrete rejection criteria: https://academy.test.io/en/articles/12829598-bug-reproduction-rejections-explained
- Submission form workflow: https://academy.test.io/en/articles/2668017-reproduction-feature
- Attachment guidance: https://academy.test.io/en/articles/2541954-bug-report-attachments

The extracted primary article omitted some list contents; exact evidence details above are grounded in the explicit rejection-criteria table. Check current instructions if platform guidance conflicts. This guide is not a timed assessment answer or evidence that a task was performed.
