# Inventory Management Database
Inventory Management Database using SQL Server with business rules and constraints.
## Current Status
- Phase 1 completed: Database schema design
- 5 tables created with constraints and relationships
- Sample data inserted
- Reporting view (BILL) created using FK → PK joins
## Tables Designed
- SUPPLIER
- PRODUCT
- STOCK
- CUSTOMER
- ORDERS
## Progress Log
- Day 1: Designed schema and implemented constraints
- Day 2: Inserted sample data and created reporting view using joins
- Join & Dependency Logic (Key Learning)

This project follows a relationship-driven approach to building SQL joins.

Instead of joining tables by guessing column names, joins are created by first identifying:

Primary key tables (independent/master)

Foreign key tables (dependent)

The bridge table that connects entities

In this schema, ORDERS acts as the bridge between CUSTOMER and PRODUCT.
All joins are built using the rule:

Always join Foreign Key → Primary Key

This approach makes multi-table joins predictable, scalable, and easy to reason about — even when working with databases designed by someone else.

## Next Steps
- Add indexes for performance optimization
- Write inventory and reorder alert queries
