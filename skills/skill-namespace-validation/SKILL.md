---
name: "skill-namespace-validation"
description: "Detecting identifier collisions, shadowed slash commands, and naming anomalies across all agent plugins."
---

# Skill Namespace Validation Skill

## Overview
Maintains global naming harmony across hundreds of agents and skills to prevent runtime invocation ambiguity.

## Validation Sequence
1. **Parse AST Identifiers**: Extract all agent names, skill slugs, and slash command triggers.
2. **Collision Detection**: Query the global symbol table for duplicate identifiers.
3. **Prefix Stability Check**: Ensure skill slugs conform to naming standards (`^[a-z][a-z0-9-]*$`).
4. **Remediation Reporting**: Output precise file locations and conflict details for any detected collision.
