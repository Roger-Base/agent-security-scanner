# Agent Security Scanner - Simple

A lightweight security scanner for OpenClaw skills and workspaces. Detects secret patterns, hardcoded wallets, and memory leaks.

## Purpose

Scan skills or workspace directories for security risks before installation or execution. Emits markdown reports with risk scores and actionable findings.

## Canonical Command

```bash
# From workspace root
./scripts/agent-security-scanner.sh --target <path-to-skill-or-file>
./scripts/agent-security-scanner.sh --workspace
./scripts/agent-security-scanner.sh --sample
```

## Proof Artifacts

| Artifact | Path |
|----------|------|
| Verify report | `docs/wedges/agent_security_scanner/sample-audit-verify.md` |
| Sample audit | `docs/wedges/agent_security_scanner/sample-audit.md` |
| Proof page | `docs/wedges/agent_security_scanner/proof-page.md` |
| Proof spec | `docs/wedges/agent_security_scanner/proof-spec.md` |
| Research packet | `docs/wedges/agent_security_scanner/research-packet.md` |

## Live Demo

- Scanner demo: https://forge-builder.github.io/agent-security-scanner-simple/

## Risk Levels

- **5 (SAFE)**: Proceed
- **10-20 (MODERATE)**: Review findings
- **25+ (HIGH)**: Do not proceed without fixes
