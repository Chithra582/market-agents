---
name: "plugin-catalog-curation"
description: "Curating, categorizing, and validating modular agentic plugins across 94 domain collections."
---

# Plugin Catalog Curation Skill

## Overview
Coordinates the ingestion, categorization, and quality auditing of multi-domain agent plugins.

## Operational Workflow
1. **Analyze Plugin Layout**: Verify that each plugin directory contains `plugin.json`, `agents/`, `skills/`, and `commands/`.
2. **Validate Metadata**: Ensure accurate category tagging, author metadata, and license specifications.
3. **Dependency Check**: Audit external tool dependencies and MCP server declarations.
4. **Catalog Indexing**: Register approved plugins into the primary `marketplace.json` catalog.
