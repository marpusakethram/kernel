---
description: Write a one-page investment-committee memo on a startup's technical moat
argument-hint: "<owner/repo | github URL | local path> [competitor repos...]"
---

# /memo

The first item in `$ARGUMENTS` is the company; any further items are competitors.

1. Call the Kernel MCP server's `audit_repository` tool on the company.
2. If competitors were given, call `compare_repositories` on the company plus its competitors.
3. Write a one-page IC memo with these sections: **Verdict**, **What is proprietary**, **What is rented** (vendor APIs, scaffolding), **Rebuild cost**, **Versus competitors** (only if compared), **Risks**, **Questions to resolve before investing**.

Use the tool numbers; do not invent metrics.

4. If a GBrain MCP server is connected (tools from the `gbrain` server), save the memo to the company's page in the brain: search for the company first and add to its existing page, or create one if there is none. Then say in one line where you saved it. If GBrain is not connected, skip this step without mentioning it.
