---
name: sql-databases
description: Guidance for SQL queries, relational schema design, migrations, transactions, and database performance. Use for database-related tasks.
---

# SQL and Relational Databases

- Identify the database engine and version; SQL dialects and features differ.
- Inspect the existing schema, constraints, indexes, relationships, and callers before changing data structures.
- Preserve data integrity with appropriate primary keys, foreign keys, unique constraints, checks, and transactions.
- Parameterize application queries; never interpolate untrusted values into SQL.
- Before destructive or irreversible operations, explain impact and require appropriate confirmation.
- Design migrations to match the project's deployment and rollback practices.
- Consider query plans and representative data before adding indexes or rewriting performance-sensitive queries.
- Avoid speculative indexes, denormalization, or schema complexity without evidence.
- Test queries against the target engine where possible. Clearly label unverified dialect assumptions.
- For PostgreSQL, use PostgreSQL documentation and features only when the actual target is PostgreSQL.
