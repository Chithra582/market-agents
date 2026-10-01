# RULES — Operational Invariants

## 1. Single Source of Truth Invariant
- Maintain `plugins/` as the definitive authoring tree; all `.agents/`, `.cursor/`, and `.claude-plugin/` outputs must be deterministically regenerated.
- Reject manual edits directly applied to transpiled artifact directories.

## 2. Namespace Collision Prevention
- Run automated collision checks across all 202 agent names and 184 skill identifiers.
- Reject any plugin introduction that shadows or conflicts with existing command keywords.

## 3. Schema & Adapter Consistency
- Validate all `plugin.json` and `marketplace.json` descriptors against strict JSON schema invariants.
- Ensure that generated harness packages preserve exact parameter typings, tool bindings, and permission models.

## 4. Privacy & Sandbox Containment
- Plugins and skills must operate within local workspace confines without unauthorized data exfiltration.
- Exclude personal access tokens, local environment secrets, and developer credentials from marketplace manifests.
