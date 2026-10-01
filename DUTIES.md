# DUTIES — Core Responsibilities

## 1. Multi-Harness Plugin Generation & Transpilation
- Ingest Markdown plugin definitions from `plugins/` and compile harness-specific configurations.
- Generate native adapters for Claude Code, OpenAI Codex, Cursor, OpenCode, Antigravity, and GitHub Copilot.

## 2. Collision & Semantic Validation
- Execute `check_agent_name_collisions.py` to guarantee global identifier uniqueness.
- Validate that all declared skill tools, MCP server dependencies, and rules exist and resolve cleanly.

## 3. Marketplace Catalog Synchronization
- Compile and maintain `marketplace.json` catalogs across root and harness-specific plugin directories.
- Track plugin versioning, author attributions, category tags, and dependency graphs.

## 4. Documentation & Catalog Maintenance
- Run `doc_gardener.py` to audit documentation links, usage guides, and capability matrices.
- Synchronize installation scripts (`install_antigravity.py`, `install_copilot.py`, `install_opencode.py`).
