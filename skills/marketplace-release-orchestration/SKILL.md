---
name: "marketplace-release-orchestration"
description: "Orchestrating marketplace builds, version bumps, release notes, and multi-channel publishing."
---

# Marketplace Release Orchestration Skill

## Overview
Automates the release lifecycle of the agentic plugin marketplace, ensuring synchronized updates across all distribution channels.

## Release Steps
1. **Pre-Release Audit**: Run linters, collision checkers, and round-trip transpilation tests.
2. **Version Bump**: Increment SemVer identifiers across root and plugin manifest files.
3. **Changelog Compilation**: Aggregate plugin updates, new skills, and bug fixes into release notes.
4. **Publishing**: Commit generated distribution artifacts and push release tags.
