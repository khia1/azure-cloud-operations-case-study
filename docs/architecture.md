Azure Architecture Overview


1. Subscription Context

This case study was implemented within a single Azure subscription used for learning and operational simulation.
The objective was to model real-world cost governance and lifecycle management practices in a controlled environment.

The subscription contained:

Resource Group: rg-cost-ops-lab

Virtual Machine (Linux-based)

Managed Disks

Azure Cost Management Budget

Azure Monitor Alerts



2. Resource Group Design

All resources were grouped under a single dedicated resource group to simulate production isolation and simplify lifecycle cleanup.

Resource Group Structure:

Virtual Machine

Network Interface

Public IP

Managed Disk

Budget configuration

Alert rules

Using a dedicated resource group enabled:

Controlled cost tracking

Centralized deletion

Resource lifecycle validation

Reduced risk of orphaned components



3. Budget Configuration Strategy

A monthly budget of CA$20 was configured under Azure Cost Management.

Alert thresholds were set at:

50% usage

80% usage

100% usage

This multi-threshold approach ensures:

Early visibility into abnormal consumption

Escalation path before overage occurs

Full limit notification at 100%

Alerts were configured to trigger email notifications for operational awareness.



4. Monitoring and Detection

Cost spike detection occurred through:

Azure Cost Analysis dashboard review

Budget alert notification

Usage trend monitoring

The virtual machine remained provisioned longer than expected, generating continuous compute charges.



5. Remediation Architecture Flow

Identify cost spike via Cost Analysis.

Validate active resources in Resource Group.

Stop and delete virtual machine.

Confirm managed disk deletion.

Verify removal of network resources.

Reassess subscription cost projection.

This structured remediation ensures no residual billing artifacts remain.



6. Preventive Controls

After remediation, the following controls were implemented:

Budget monitoring with tiered alerting

Manual lifecycle verification checklist

Ongoing monthly cost review practice

Resource cleanup validation before project closure



7. Architectural Lessons

Key design takeaways:

Small subscriptions can still incur unexpected costs.

Resource groups are critical for cost isolation.

Budget alerts must be implemented before workload testing.

Deleting VMs does not always delete attached disks automatically.

Governance must be proactive, not reactive.


## Architecture Overview

User / Dev
↓
Azure Subscription
↓
Resource Group
↓
Virtual Machine
↓
Cost Monitoring (Azure Cost Management + Alerts)

