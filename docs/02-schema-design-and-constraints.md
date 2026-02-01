# 02 — Schema Design and Constraints

## Goal
Use relational constraints to enforce integrity under concurrency.

## Constraints (Conceptual)
- primary keys and natural keys where appropriate
- unique constraints for idempotency keys
- foreign keys for referential integrity
- CHECK constraints for enum-like fields

## Transaction Rules
- order placement and fills are atomic
- write receipts before updating projections
- avoid partial updates by using single-transaction commits
