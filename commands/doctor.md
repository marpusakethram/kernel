---
description: Check that Kernel is installed and scoring correctly
---

# /doctor

Verify the install the way `gbrain doctor` does: run the real engine on known inputs and check the answer.

1. Call the Kernel MCP server's `run_benchmarks` tool.
2. It scores four built-in sample startups. **Pass** only if all four come back and their Real Tech Scores rise in this order:
   `ai-pdf-chat-wrapper` (Wrapper) < `b2b-invoice-saas-crud` (Standard app) < `hyper-crdt-sync-engine` (Real engine) < `nova-bytecode-vm-kernel` (Deep tech).
   With default settings the scores are 2, 12, 28 and 53. The order is what matters.
3. Reply in one short block: `Kernel doctor: PASS` or `Kernel doctor: FAIL`, then the four scores in order.

If the tool is missing or errors, report FAIL with the likely fix:
- Node 18 or newer must be on your PATH (`node --version`).
- Then run `/plugin update kernel@kernel`, or reinstall, and restart Claude Code.
