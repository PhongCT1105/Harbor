# Discovery

## Purpose
Explain how discovery fits into Harbor's control-plane responsibilities.

## Scope
This file should describe what Harbor needs to learn about MCP servers and tools without specifying discovery mechanisms.

## Project Pillars
- MCP Server Management: discovery should help Harbor build an accurate view of registered servers, their metadata, and available tools.
- Tool Calling Accuracy: discovery should provide the capability information needed for later filtering, routing, and ranking.

## Intended Audience
- Contributors
- Users
- Plugin developers
- Core maintainers
- AI coding agents

## Planned Sections
- Discovery overview
- Discoverable entities
- Discovery lifecycle
- Relationship to registry
- Relationship to tool selection

## TODO
- [ ] Define discovery terminology.
- [ ] Document discovery goals and boundaries.
- [ ] Link future design work for server and tool indexing.
