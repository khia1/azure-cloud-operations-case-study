# Azure Cost Incident Report

## Executive Summary
During February 2026, an unexpected cost spike of approximately CA$200 was observed in an Azure subscription.

## Root Cause
A virtual machine was provisioned and left running without predefined cost governance controls or alert thresholds.

## Impact
Temporary billing overage requiring support intervention.

## Detection
The issue was identified via Azure Cost Analysis after reviewing accumulated monthly spend.

## Remediation Steps
- Contacted Azure Support and verified billing adjustment
- Deleted the running virtual machine
- Confirmed removal of associated managed disks
- Implemented monthly budget (CA$20) with alerts at:
  - 50%
  - 80%
  - 100%

## Preventive Controls Implemented
- Budget monitoring and alert configuration
- Resource lifecycle cleanup verification process
- Ongoing cost analysis monitoring

## Lessons Learned
Proactive budget controls and lifecycle discipline are essential to prevent cost leakage in cloud environments.
