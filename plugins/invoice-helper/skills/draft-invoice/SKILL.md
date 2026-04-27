---
description: Draft a client invoice from a short summary of completed work
disable-model-invocation: true
---

# Draft Invoice

The user will provide a short summary of work performed for a client (project name, dates, hours or deliverables, hourly rate or fixed fee). Produce a clean, plain-text invoice draft they can paste into their invoicing tool.

Include:
- A header line: client name, invoice date (today), and a placeholder invoice number (`INV-YYYYMMDD-001`).
- Itemised lines: description, quantity (hours or units), unit rate, line total.
- Subtotal, tax line (left at 0 unless the user mentions a tax rate), and total.
- Payment terms (default: Net 14) and a payment method placeholder.

If any of the inputs above are missing, ask one consolidated question listing only the missing fields — do not ask one question at a time. After the user answers, produce the invoice without further confirmation.

User input: $ARGUMENTS
