---
description: Real tech or wrapper? Audit a startup's codebase and get a verdict, Moat Score and founder questions
argument-hint: "<owner/repo | github URL | local path | benchmark:vm>"
---

# /audit

Audit the codebase given in `$ARGUMENTS` with the Kernel MCP server's `audit_repository` tool.

If `$ARGUMENTS` is empty, audit the current working directory (pass its absolute path as the target).

Then answer like a sharp investor, in this order:

1. **Verdict in one sentence** — the plain-English tier (Wrapper, Standard app, Real engine, Deep tech) and the Real Tech Score out of 100.
2. **Moat Score and grade**, with the two or three metrics that drove it (engine size and rebuild cost, vendor independence, integrity, engine depth, tests).
3. **Where the real engineering lives** — the top engine files, and what each one appears to do (open the top file if it helps you describe it).
4. **Red flags** — rented AI/API dependence, dense code nothing uses, missing tests.
5. **Questions to ask the founder** — use the tool's questions; keep the best four.

Keep it under 250 words unless the user asks for more. Scores rank companies against each other; do not present them as absolute grades.

## Save it to the brain

If a GBrain MCP server is connected (tools from the `gbrain` server), file this audit on the company's page: search the brain for the company first and add to its existing page, or create a page for it if there is none. Record the date, the repo checked, the verdict, the Real Tech and Moat scores, the red flags and the founder questions. Then say in one line where you saved it. If GBrain is not connected, skip this section without mentioning it.
