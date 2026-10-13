# Issue and PR Tracker

Record each candidate's status, overlap check, and evaluation. Recheck GitHub immediately before starting and before submitting a PR.

[日本語版](TRACKER.ja.md)

| Status | Repository / Issue | Summary | Overlap check | Assessment | Next action |
| --- | --- | --- | --- | --- | --- |
| Excluded | [agent-chat-ui#290](https://github.com/langchain-ai/agent-chat-ui/issues/290) | Change SVG `clip-path` to React's `clipPath` | PRs #273, #296, and #315 include the same fix (checked 2026-10-13) | Small, but duplicated | Do not start |
| On hold | [agent-chat-ui#327](https://github.com/langchain-ai/agent-chat-ui/issues/327) | KaTeX version mismatch | The issue points to PR #326 (checked 2026-10-13) | Small, but an existing solution is proposed; current PR status still needs checking | Wait until #326 is resolved |

## Status definitions

- `Candidate`: under evaluation; work has not started.
- `Awaiting confirmation`: waiting for the maintainer or reviewer.
- `In progress`: overlap was rechecked and the approach is agreed.
- `Human review`: a diff is ready for your first review.
- `Approved to submit`: you approved the submission.
- `PR submitted`: an upstream PR has been opened.
- `Complete`: merge or closure outcome and lessons are recorded.
- `Excluded` / `On hold`: not proceeding; record the reason.
