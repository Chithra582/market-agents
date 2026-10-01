---
name: "cross-harness-transpilation"
description: "Compiling source Markdown definitions into native artifacts for Claude Code, Cursor, Codex, and Antigravity."
---

# Cross-Harness Transpilation Skill

## Overview
Transforms canonical Markdown plugin definitions into harness-idiomatic configurations without semantic loss.

## Transpilation Pipeline
1. **Source Ingestion**: Parse canonical plugin definitions from `plugins/`.
2. **Adapter Mapping**: Apply harness-specific transformation rules (Cursor `.cursorrules`, Antigravity skills, Codex prompts).
3. **Artifact Generation**: Emit cleanly structured target directories (`.agents/`, `.cursor/`, etc.).
4. **Parity Verification**: Run regression suites to ensure equivalent tool execution behavior across harnesses.
