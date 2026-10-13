# AI OSS Job Hunt

An AI-led open-source contribution project. The AI proactively searches for useful issues, evaluates whether it can make a responsible contribution, and prepares focused changes. Human review adds judgment, context, and accountability before anything is submitted upstream.

“Job hunt” is a metaphor for the AI taking initiative to find meaningful work. The project is about responsible collaboration between AI and human reviewers.

[日本語版はこちら](README.ja.md)

## How it works

- The AI proactively discovers open issues that may benefit from a contribution.
- It studies the issue, repository guidance, relevant code, duplicate pull requests, and maintainer expectations.
- It proposes a focused change and explains its reasoning, risks, and verification.
- A human reviews the issue choice and proposed change, adding context and requesting revisions where needed.
- External comments and pull requests are submitted only after human review and explicit approval.
- Outcomes, including rejected or abandoned proposals, are recorded transparently.

## Workflow

1. The AI searches for candidates using the [issue selection criteria](docs/issue-selection.md).
2. It records candidates and overlap checks in the [issue and PR tracker](TRACKER.md).
3. It explains the issue, reproduction steps, expected behavior, and acceptance criteria.
4. It prepares a focused change and reports scope, risks, and verification results.
5. A human reviews the proposal using the [review workflow](docs/review-workflow.md).
6. After explicit approval, the AI may submit a comment or PR to the upstream project.
7. The AI records the outcome and lessons in the [activity log](ACHIEVEMENTS.md).

## Principles

- Make candidate discovery AI-led and proactive.
- Check for duplicate work before starting and again before submitting.
- Keep changes focused on the issue's stated purpose.
- Explain reasoning and disclose anything not verified.
- Use human review to add judgment and catch errors; do not submit externally without explicit approval.
- Represent AI and human contributions accurately.
- Record unsuccessful attempts and lessons learned.

## Project files

- `docs/issue-selection.md` — how candidate issues are evaluated
- `docs/review-workflow.md` — how AI work is presented for human review
- `TRACKER.md` — candidate issues and progress
- `ACHIEVEMENTS.md` — contributions, outcomes, and lessons

## Current candidates

[langchain-ai/agent-chat-ui#327](https://github.com/langchain-ai/agent-chat-ui/issues/327) is a small dependency-version issue, but its description points to PR #326. It is **on hold** to avoid duplicate work. [Issue #290](https://github.com/langchain-ai/agent-chat-ui/issues/290) is excluded because multiple PRs already propose the same fix. The AI will continue searching for an issue with clear scope, no overlapping work, and a path to maintainer acceptance.
