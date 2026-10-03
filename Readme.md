# SAP Automation Projects

> **Copyright & Usage Notice**  
> Copyright © 2026 Aditya Sarkale. All rights reserved **to the extent of rights owned by the author**.  
> No license is granted to copy, modify, redistribute, publish, sublicense, or use this source code or substantial portions of it outside the GitHub platform without prior written permission from the applicable rights holder.  
> **Important:** Any company-owned, client-owned, SAP-proprietary, third-party, or otherwise restricted material remains subject to its applicable ownership, confidentiality, and licensing terms.

## Purpose
A collection of SAP automation projects covering repetitive business workflows such as outbound delivery/invoice processing, production automation, material reservation, scheduling agreements and related SAP GUI activities.

## Projects
| Project | Primary workflow |
|---|---|
| [Scheduling Agreement Automation](https://github.com/AdiSarkale/Scheduling-Agreement-Automation-in-SAP) | ME38 scheduling-agreement processing |
| [Transfer Posting SAP](https://github.com/AdiSarkale/Transfer-Posting-SAP) | Material transfer posting |
| [SAP Production Automation & Material Reservation](https://github.com/AdiSarkale/SAP-Production-Automation-and-Material-Reservation) | CO11N / MB21 / VL01N workflows |
| [Outbound Delivery & Invoice Automation](https://github.com/AdiSarkale/Outbound-Delivery-and-Invoice-Process-Automate) | Delivery, invoice and related processing |

## Common Architecture
Most applications follow this pattern:
```
Web UI / Input File
       ↓
Python / Flask
       ↓
pywin32 / SAP GUI Scripting
       ↓
SAP transaction
       ↓
Status / result
```

## Common Prerequisites
- Windows
- SAP GUI for Windows
- SAP GUI Scripting enabled on client
- Server-side scripting enabled by SAP Basis where required
- Python
- Node.js for React-based frontends
- Appropriate SAP authorization

## Common Troubleshooting
### SAP not logged in / User cancelled
1. Confirm SAP GUI is logged in.
2. Check the active scripting session.
3. Open RZ11.
4. Verify the relevant dynamic scripting parameter is **TRUE**.
5. Escalate server configuration issues to SAP Basis.

### Website inaccessible
Use the organization's approved internal server procedure. Internal server names, credentials and operational secrets are intentionally excluded from this public documentation.

## Development Rules
- Do not commit credentials or secrets.
- Do not commit confidential company data.
- Test SAP automation in a controlled environment before production execution.
- Keep project-specific README files updated when workflows change.

## Author
**Aditya Sarkale** — https://github.com/AdiSarkale
