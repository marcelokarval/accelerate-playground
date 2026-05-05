# Accelerate Playground

This repository is a persistent GitHub playground for **Accelerate** live workflow tests.

It exists so Accelerate can safely exercise and verify GitHub-facing actions such as:

- repository discovery;
- branch creation and push;
- pull request creation;
- pull request lookup/rehydration;
- artifact/comment attachment;
- closure/readiness proof flows;
- future workflow-adapter tests from other sessions and other projects.

## Intended Use

This repository may be reused by future agent sessions, Accelerate sessions, and related project experiments.

It is intentionally low-stakes and should not contain production code, private data, secrets, credentials, customer data, or proprietary material.

## Persistence Policy

Do **not** delete this repository at the end of a test run.

Keeping it around is part of the contract: it provides durable remote state for validating that Accelerate can confirm its own GitHub actions across sessions.

## Safety Rules

- Test branches and pull requests are allowed.
- Test comments and generated proof artifacts are allowed.
- Destructive operations should be avoided unless a future test explicitly documents why they are safe.
- Secrets and sensitive data are prohibited.

## Current Owner

- GitHub owner: `marcelokarval`
- Primary purpose: Accelerate remote-provider proof playground
