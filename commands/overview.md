---
description: Show a high-level Gardera security overview of the organization.
---

Call the `get_organization_overview` tool from the `gardera` MCP server, then summarize the response as a short bulleted list. Aim for 4–5 bullets total. Each bullet is a complete sentence written in natural prose. Not a "label: value" pair. Group related facts together so each bullet covers a single theme:

- One bullet for org-wide totals: repository count, cloud account/project count and open findings, with the severity breakdown (critical, high, medium, low) folded into the same sentence.
- One bullet on SLA: the over-SLA count with per-finding-type breakdown in parentheses, and any close-to-breach items mentioned in the same sentence. Omit the bullet entirely if everything is zero.
- One bullet for the top 3 teams by open finding count.
- One bullet summarising action-center items worth attention. Skip individual items that are zero or null. Omit the whole bullet if nothing is worth flagging.

Add light interpretive framing where it helps the reader (e.g. "SLA health is the main concern" or "the bulk of findings sit in Cloud Security"), but stay tight. No headers, no nested bullets, no raw JSON.
