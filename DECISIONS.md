# Architecture Decision Records

This document records important architectural decisions made during the development of SmartRoute AI.

---

## ADR-001

Decision

Use Java Spring Boot as Backend.

Reason

- Enterprise Standard
- Excellent Security
- Large Ecosystem
- High Performance

---

## ADR-002

Decision

Use PostgreSQL.

Reason

- ACID Compliance
- Complex Relationships
- Enterprise Database

---

## ADR-003

Decision

Use React.

Reason

- Component-Based
- Fast UI Development
- Large Community

---

## ADR-004

Decision

Use Graph Algorithms.

Reason

The logistics problem is naturally represented as a weighted graph.

This enables:

- Dijkstra
- A*
- BFS
- DFS
- Floyd-Warshall
- Prim
- Kruskal

---

## ADR-005

Decision

Use JWT Authentication.

Reason

Stateless Authentication

Scalable

Secure

Industry Standard