# Event Model

## Purpose
Model business activities as structured events for data-driven architecture.

## Core Event Types

- CONTRACT
- INVOICE
- CASH
- REVENUE

## Sample JSON

```json
[
  {"type":"CONTRACT","amount":1000000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-03"},
  {"type":"INVOICE","amount":1000000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-03"},
  {"type":"CASH","amount":1000000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-04"},
  {"type":"REVENUE","amount":250000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-03"}
]
```

## Vision

Move from bookkeeping to event-driven data architecture.
