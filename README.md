# Event Model

## Purpose
Model business activities as structured events for data-driven architecture.

## Core Event Types

- CONTRACT
- INVOICE
- CASH
- REVENUE

## Sample JSON

[
  {"event_id":"EVT-0001","type":"CONTRACT","amount":1000000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-03"},
  {"event_id":"EVT-0002","type":"INVOICE","amount":1000000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-03"},
  {"event_id":"EVT-0003","type":"CASH","amount":1000000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-04"},
  {"event_id":"EVT-0004","type":"REVENUE","amount":250000,"entity":"ClientA","project":"P001","unit":"Sales","month":"2026-03"}
]

## Vision

Move from bookkeeping to event-driven data architecture.

## Event Schema (v0)

Required
- type: string
- amount: number
- entity: string
- project: string
- unit: string
- month: YYYY-MM

Optional
- currency: string (default: JPY)
- event_id: string
- source: string (hubspot / freee / mf / manual)
- occurred_at: ISO datetime
- tags: string[]
