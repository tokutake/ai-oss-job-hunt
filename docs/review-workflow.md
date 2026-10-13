# Human Review Workflow

Issue discovery and initial investigation are AI-led. Human review adds context, judgment, and accountability before an external contribution is submitted.

[日本語版](review-workflow.ja.md)

## Roles

- **AI:** proactively finds candidate issues, investigates the repository, proposes a focused change, verifies it, and explains its reasoning.
- **Human reviewer:** evaluates the issue choice and proposed change, supplies context, catches errors, and decides whether the work is ready.
- **External submission:** comments or pull requests are submitted only after human review and explicit approval.

## Every review request should include

1. Issue URL and acceptance criteria
2. Why the AI selected it and how it checked duplicate PRs and maintainer expectations
3. Explanation of the cause, with relevant files and lines
4. Change summary, alternatives, compatibility, and side effects
5. Verification performed and results, including failures and anything not run
6. Full diff and decisions needing human input
7. Draft text for an upstream comment or PR

## Reviewer checklist

- Did the AI understand the issue and acceptance criteria?
- Is the change small and within scope?
- Can the AI explain what each part of the diff does and why it is needed?
- Were edge cases, types, accessibility, and security implications considered?
- Does verification match the change, with failures and omissions disclosed?
- Were the upstream contribution guide, license, CLA, and PR template checked?
- Are AI and human contributions represented accurately?

## Decision

- **Approve:** explicitly authorize the AI to submit the work upstream.
- **Request changes:** the AI revises the work, then presents the full diff for another review.
- **Pass:** if overlap, unclear reasoning, maintainer concerns, or unverifiable behavior remain, record why and continue searching.

The goal is collaborative judgment: AI takes initiative, while human review improves the quality and accountability of external contributions.
