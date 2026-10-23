---
description: X-ray one file — which lines are real engineering and which are scaffolding
argument-hint: "<target> [file]"
---

# /xray

Parse `$ARGUMENTS` as a target (owner/repo, URL, local path, or benchmark:<id>) optionally followed by a file path.

Call the Kernel MCP server's `xray_file` tool. If no file was given, call it without `file` first to list the files ranked by real engineering, then X-ray the top one.

Show the tagged listing, then explain in two or three sentences what the DECISION lines do and how much of the file is scaffolding (LAYOUT, DATA-DEF, API-RELAY, SETUP, COMMENT).
