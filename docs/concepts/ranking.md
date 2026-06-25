# Ranking

## Purpose
Explain the conceptual role of ranking in Harbor's tool-selection flow.

## Scope
This file should cover why ranking exists, what signal categories may matter, and how ranking relates to routing without defining algorithms.

## Project Pillars
- MCP Server Management: ranking should be able to consider operational signals such as availability, health, latency, errors, usage, and preferences.
- Tool Calling Accuracy: ranking should help choose relevant and reliable tools based on request fit, schema match, past outcomes, and current conditions.

## Intended Audience
- Contributors
- Users
- Plugin developers
- Core maintainers
- AI coding agents

## Planned Sections
- Ranking overview
- Ranking goals
- Signal categories
- Explainability expectations
- Relationship to tool selection

## TODO
- [ ] Define ranking terminology.
- [ ] Separate ranking goals from future algorithm choices.
- [ ] Add evaluation questions for ranking quality.
