---
title: "Confirm knowledge"
read_only: true
type: "command"
argument-hint: interaction|process|commits|tools|memory|status
---

Quick knowledge check with optional focus areas.

# Arguments:

$ARGUMENTS can include any combination of:

- `interaction` - How to communicate with you
- `process` - TDD workflow and coding approach
- `commits` - Git workflow and commit process
- `tools` - Available MCP tools and usage
- `memory` - Basic-memory tool patterns
- `status` - Current project/task state (includes basic-memory search)

If no arguments provided, only check current status unless it's unclear.

# Skip this command if:

- Already mid-task in current session
- Context clearly shows ongoing work

# Response format:

**Checking**: $ARGUMENTS or "status only"

For each requested area:

- **[area]**: ✅ [brief confirmation] | 🚨 [what's unclear]

**Current focus**: [specific task or "awaiting instructions"]
