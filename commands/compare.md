---
description: Head-to-head a startup against its competitors — who has the stronger IP and the better engine?
argument-hint: "<repo-a> <repo-b> [repo-c ...]"
---

# /compare

Compare the repositories listed in `$ARGUMENTS` (space- or comma-separated; at least two) with the Kernel MCP server's `compare_repositories` tool.

If fewer than two repositories are given, ask for the competitor repos before calling the tool.

Report:

1. **Stronger IP** — who wins and by how much, citing engine size, rebuild cost and vendor independence.
2. **Better engine** — who wins and by how much, citing Real Tech Score, engine depth, tests and integrity.
3. **The scoreboard** — the head-to-head table from the tool.
4. **What it means** — one line per company on its technical moat, calling out anyone built mostly on rented AI APIs or carrying dense code nothing uses.
