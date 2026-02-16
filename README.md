# azure-cloud-operations-case-study
Azure cost governance and cloud operations case study demonstrating budget controls, monitoring setup, and resource lifecycle management.


# Azure Cloud Operations Case Study

## Overview
This project demonstrates practical Azure cost governance and operational control in a real subscription environment.

Focus areas:
- Budget creation and alert configuration
- Cost analysis and overage investigation
- Resource lifecycle management (VM provisioning and deletion)
- Monitoring and spend control



## Scenario

A virtual machine was provisioned for testing purposes.
Unexpected costs were generated during the billing cycle.

Actions taken:
- Investigated cost breakdown in Azure Cost Analysis
- Identified primary cost driver (Virtual Machines)
- Implemented monthly budget (CA$20)
- Configured alert thresholds at 50%, 80%, and 100%
- Deleted unused virtual machine and verified resource cleanup
- Confirmed removal of managed disks



## Cost Governance Implementation

### Budget Configuration
- Monthly budget: CA$20
- Alerts:
  - 50% threshold
  - 80% threshold
  - 100% threshold

### Monitoring Tools Used
- Azure Cost Analysis
- Resource Group inspection
- Virtual Machine lifecycle management
- Disk validation



## Lessons Learned

- Azure resources continue billing while provisioned
- Budget alerts are essential for cloud cost control
- VM deletion must include disk validation
- Cost analysis provides clear service-level breakdown



## Skills Demonstrated

- Azure subscription management
- Cloud cost governance
- Operational monitoring
- Incident response to unexpected billing
- Resource cleanup verification



## Tools

- Microsoft Azure Portal
- Azure Cost Management
- GitHub documentation
