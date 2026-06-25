# Cache

## Purpose
Explain the conceptual role of caching in Harbor.

## Scope
This file should describe what kinds of information may be cacheable and why caching matters for control-plane and runtime behavior.

## Project Pillars
- MCP Server Management: caching may help Harbor keep server and tool information available while still respecting freshness.
- Tool Calling Accuracy: caching may reduce repeated work for tool discovery, selection context, and other accuracy-supporting signals.

## Intended Audience
- Contributors
- Users
- Plugin developers
- Core maintainers
- AI coding agents

## Planned Sections
- Cache overview
- Cacheable information categories
- Freshness concepts
- Relationship to discovery
- Relationship to execution

## TODO
- [ ] Define caching terminology.
- [ ] Document freshness questions.
- [ ] Identify future invalidation and consistency topics.
