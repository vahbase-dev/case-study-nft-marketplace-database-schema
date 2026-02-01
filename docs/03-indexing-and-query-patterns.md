# 03 — Indexing and Query Patterns

## Goal
Support hot queries with stable latency at scale.

## Hot Queries (Examples)
- latest trades per collection
- active listings by price and rarity
- user portfolio and activity feed
- order book views and recent fills

## Index Strategy
- composite indexes aligned to filters + sort order
- partial indexes for active states
- materialised views / denormalised tables for read-heavy paths
