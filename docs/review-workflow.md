# Human Review Workflow

The AI finds candidate issues and prepares changes. You act as hiring manager and first reviewer.

[日本語版](review-workflow.ja.md)

## Roles

- **AI (applicant):** researches the issue and code, explains why it chose the task, prepares a focused fix, verifies it, and drafts an upstream proposal.
- **You (reviewer):** check the issue understanding, approach, diff, and verification, then decide whether it may be submitted.
- **External submission:** the AI may comment or open a PR only after your review and explicit approval.

## Every review request should include

1. Issue URL and acceptance criteria
2. Why the AI selected it and how it checked for duplicate PRs and maintainer expectations
3. Explanation of the cause, with relevant files and lines
4. Change summary, alternatives, compatibility, and side effects
5. Verification performed and results, including failures and anything not run
6. Full diff and any decisions needing your input
7. Draft text for an upstream comment or PR

## Reviewer checklist

- Did the AI understand the issue and acceptance criteria?
- Is the change small and within scope?
- Can the AI explain what each part of the diff does and why it is needed?
- Were edge cases, types, accessibility, and security implications considered?
- Does the verification match the change, with failures and omissions disclosed?
- Were the upstream contribution guide, license, CLA, and PR template checked?
- Does the proposal clearly describe this as AI-generated work?

## Decision

- **Approve:** explicitly ask the AI to submit the work upstream.
- **Request changes:** the AI revises the work, then presents the full diff for another review.
- **Pass:** if overlap, unclear reasoning, maintainer concerns, or unverifiable behavior remain, record why and look for another candidate.

AI output is not presumed correct. The experiment tests whether AI can own its reasoning and explanation as well as its deliverable.
