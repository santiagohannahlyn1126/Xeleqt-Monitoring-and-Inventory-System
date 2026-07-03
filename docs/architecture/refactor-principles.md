# Refactor Preservation Principles

## Non-negotiable guarantees

- Preserve all existing working features, designs, routes, dashboards, modals, tables, filters, animations, light/dark mode behavior, and user flows.
- Refactor internal architecture without replacing the existing UI with a generic redesign.
- Keep the original repository unchanged as the reference implementation.
- Preserve valid legacy data and flag unmappable records for review rather than deleting them.

## Refactor priorities

1. Stop destructive initialization and unsafe stock operations.
2. Introduce versioned migrations.
3. Normalize PO, BOM, inventory, stock, transfer, and manufacturing data.
4. Separate routing, controllers, services, repositories, validation, and audit logging.
5. Implement authenticated user identity and role enforcement.
6. Keep compatibility adapters until all preserved UI flows use the corrected APIs.

## Supported roles

- ADMIN
- HARDWARE_EMPLOYEE
- FINANCE
- MANUFACTURING_COMPANY

There is no supplier user role.

## Approval rule

Approval status is limited to PENDING and APPROVED. PENDING requires a reason. Shipment, production, quality, and lifecycle states use separate status domains.
