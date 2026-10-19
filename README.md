# agent-receipts

Check what your AI agent claimed against what it actually did.

## Why

Agents report work they never did: "tests pass" when no test ran, a sourced briefing with claims that no fetched page supports, a loop that says "done" after it quietly gave up. The transcript holds the truth, but nobody reads it against the output.

## What it does

agent-receipts reads an agent's session transcript or trace and:

1. extracts what the agent claimed (it ran the tests, it verified something, a fact came from a source)
2. looks for the tool call, fetched page or trace step that backs each claim
3. reports each gap with the line of the transcript where it happened

## Status

In active development. The first version targets Claude Code session transcripts and research-agent traces. A tagged v0.1 with one-command install is planned for November 2026.
