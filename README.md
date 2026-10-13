# AI OSS Job Hunt

A half-joke, half-serious experiment: can an AI find open-source work, make a useful contribution, and earn the trust of maintainers? The AI searches for issues, studies the code, prepares a change, and reports both results and failures. You are the hiring manager and first reviewer.

[日本語版はこちら](README.ja.md)

## What “job hunting” means here

- The AI finds open issues as potential work.
- It checks the issue, existing code, duplicate pull requests, and maintainer expectations before choosing a task.
- It prepares a focused change and explains the reasoning and verification.
- You review the first submission and decide whether it is ready.
- After your approval, the AI submits the contribution upstream and records the maintainers’ response.

This project does not automate a human job search. It tests whether an AI can find work, deliver responsibly, and explain its decisions.

## Workflow

1. The AI evaluates candidates using the [issue selection criteria](docs/issue-selection.md).
2. It records candidates and duplicate checks in the [issue and PR tracker](TRACKER.md).
3. It explains the issue, reproduction steps, expected behavior, and acceptance criteria.
4. It prepares a small change and reports scope, risks, and verification results.
5. You review it using the [review workflow](docs/review-workflow.md).
6. Only after your explicit approval does the AI comment on or submit a PR to an external project.
7. The AI records acceptance, rejection, revision requests, and lessons in [activity log](ACHIEVEMENTS.md).

## Principles

- Check for duplicate work before starting and again before submitting.
- Keep the first contribution focused on one issue and one purpose.
- Explain the reasoning and disclose anything not verified.
- Do not submit externally without your review and explicit approval.
- Describe the work honestly as an AI-led experiment.
- Record unsuccessful attempts and what the AI learned.

## Project files

- `docs/issue-selection.md` — how the AI evaluates candidate issues
- `docs/review-workflow.md` — how the AI presents work for human review
- `TRACKER.md` — candidate issues and progress
- `ACHIEVEMENTS.md` — applications, contributions, outcomes, and lessons

## Current candidates

[langchain-ai/agent-chat-ui#327](https://github.com/langchain-ai/agent-chat-ui/issues/327) is a small dependency-version issue, but its description points to PR #326. It is **on hold** to avoid duplicate work. [Issue #290](https://github.com/langchain-ai/agent-chat-ui/issues/290) is excluded because multiple PRs already propose the same fix. The AI will look for another candidate and check for overlap and maintainer acceptance before starting.
