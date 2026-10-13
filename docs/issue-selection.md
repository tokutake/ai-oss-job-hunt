# Issue Selection Criteria

Score each candidate from 0 to 2 on every criterion: 2 means clearly suitable, 1 means more information is needed, and 0 means unsuitable.

[日本語版](issue-selection.ja.md)

| Criterion | A score of 2 means |
| --- | --- |
| Acceptance | The issue is open, outside contributions are welcome, and any needed maintainer agreement is in place |
| Low overlap | No open PR addresses the same change, and recent merges have not already fixed it |
| Small scope | The work can be limited to one behavior, display, or documentation change |
| Reproducibility | Steps, environment, and expected behavior can be verified |
| Clear change | The affected area and acceptance criteria are clear and need little design judgment |
| Verifiability | Existing project commands or a clear manual check can confirm the result |
| Learning value | The AI can explain the relevant technology and code path |

**Target:** 10 or more points, with 2 points for both Acceptance and Low overlap. Any zero means hold or reject the candidate and record why.

## Hold or reject when

- An open PR fixes the same problem, or the fix is already on the default branch.
- The issue is closed, stale, abandoned, or maintainers say they are handling it.
- It is a question, broad feature request, or large design change unsuitable for a first contribution.
- It cannot be reproduced and needs more information from the reporter or maintainers.
- The change touches high-impact security, billing, or authentication behavior the AI cannot confidently assess.
- License, CLA, or contribution policy requirements remain unclear.

## Research checklist

1. Read the issue state, body, comments, labels, and last-updated date.
2. Search open PRs by issue number, symptom, function, and file names.
3. Check closed and merged PRs for an existing fix.
4. Inspect recent changes on the default branch and the relevant code.
5. Recheck immediately before starting and record the date in the tracker.

Scores help compare candidates. They do not override maintainer guidance or repository rules.
