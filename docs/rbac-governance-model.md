Note: All resource names used in this document are illustrative and do not represent live environments.


# Azure RBAC Governance Model

## Objective

Demonstrate role-based access control implementation in Azure to enforce least-privilege principles and reduce operational risk.

---

## Scenario

A development team requires access to deploy and manage virtual machines, but should not have permission to modify billing settings or delete resource groups.

---

## Risk Without RBAC

- Accidental deletion of production resources  
- Unauthorized billing changes  
- Excessive privilege exposure  
- Compliance violations  

---

## RBAC Strategy

### Roles Assigned

- Contributor role for development team on specific resource group
- Reader role for finance team on subscription level
- Owner role restricted to Cloud Administrator

---

## Implementation Steps

1. Created resource group: `rg-example-production`
2. Assigned Contributor role to DevOps group at resource group scope
3. Verified effective permissions
4. Audited access via Azure Activity Log

---

## Validation

- Developer account successfully deployed VM
- Developer account could NOT delete resource group
- Billing settings remained restricted

---

## Operational Impact

This model enforces least privilege access and reduces risk of accidental or malicious misconfiguration.

RBAC implementation strengthens governance and aligns with enterprise security standards.
