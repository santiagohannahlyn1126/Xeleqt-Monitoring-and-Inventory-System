# Xeleqt Monitoring and Inventory System

Refactored successor of `Xeleqt-Inventory-Monitoring-System`.

## Refactor guarantees

- Preserve all existing working features, designs, routes, dashboards, modals, tables, filters, and user flows.
- Correct database, API, authentication, stock, BOM, PO, manufacturing, transfer, and audit mismatches.
- Use normalized relational data, versioned migrations, domain-based file organization, and immutable stock history.
- Keep the original repository unchanged as the reference implementation.

## Target domains

- Authentication and users
- Dashboard
- Inventory and components
- Purchase orders
- Bill of materials
- Stock containers and movements
- Transfers and usage
- Manufacturing
- Reports and audit
- Settings

## Migration policy

No existing valid record should be silently deleted. Legacy data that cannot be mapped safely must be preserved and flagged for review.
