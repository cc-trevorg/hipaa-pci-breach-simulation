# hipaa-pci-breach-simulation
Simulated HIPAA/PCI breach lab: OSINT and phishing on a remote sysadmin yield VPN credentials, then lateral movement across a flat VPC into a private SQL subnet holding PII and card data. Covers attacker path, missed detections, and remediation.
## Table Of Contents 
### - [1. Scenario & Scope](#1-scenario--scope)
### - [2. Environment Architecture (Terraform)](#2-environment-architecture-terraform)
### - [3. Stage 1 - OSINT & Target Selection](#3-stage-1--osint--target-selection)
### - [4. Stage 2 - Phishing & Initial Access](#4-stage-2--phishing--initial-access)
### - [5. Stage 3 - Credential Harvest & VPN Entry](#5-stage-3--credential-harvest--vpn-entry)
### - [6. Stage 4 - Lateral Movement Across a Flat VPC](#6-stage-4--lateral-movement-across-a-flat-vpc)
### - [7. Stage 5 - Database Access & Exfiltration](#7-stage-5--database-access--exfiltration)
### - [8. Why Nothing Alerted](#8-why-nothing-alerted)
### - [9. Detection Engineering - Closing the Gap](#9-detection-engineering--closing-the-gap)
### - [10. Remediation (Terraform diffs)](#10-remediation-terraform-diffs)
### - [11. Compliance Mapping - HIPAA & PCI DSS](#11-compliance-mapping--hipaa--pci-dss)
### - [12. Cost of the Lab](#12-cost-of-the-lab)