# endpoint-portfolio
Endpoint platform case studies: MECM/SCCM OSD, Intune + Apple Business Manager/VPP, Okta identity controls, PowerShell/Python automation, REST API integrations, and change-control practices.


Scott Wells — Endpoint Engineering Portfolio (Sanitized)

I build and operate endpoint platforms that are secure, scalable, and supportable. My work focuses on automation, change control, compliance posture, and making deployments boring (the highest compliment in IT). Below are representative projects, sanitized to avoid proprietary details.

1) Enterprise Endpoint Migration & OSD Platform (2,500+ endpoints)

Problem: Consolidate and standardize Windows endpoint deployment at scale while keeping users productive during transition.

Scope: Domain-joined Windows 10/11 imaging + application deployment for 2,500+ endpoints, multi-team delivery, high operational risk.

Approach:

Stood up an SCCM/SQL lab in two weeks to validate changes before production.

Stabilized production SCCM, packaged OSD apps, and created a standardized OSD image.

Led three contractor workstreams (Imaging/Deployment, App Packaging, SCCM Administration).

Served as sole OSD architect; ran legacy and new laptops in parallel and executed staged cutovers.

Built repeatable deployment practices: verification steps, rollback thinking, and documentation.

Outcome:

Delivered staged cutovers with zero user-visible business disruption during endpoint migration.

Improved reliability and repeatability of deployment processes across teams.

Tools: MECM/SCCM, Windows ADK/OSD, SQL, GPO/AD, documentation/runbooks

2) Security & Compliance Controls + “Day-One Manageability” Connectivity

Problem: Improve endpoint security posture and audit readiness while ensuring devices remain manageable from first boot (not after users “remember to VPN”).

Scope: Fleet-wide endpoint and identity control implementation aligned to regulated expectations.

Approach:

Implemented Absolute Persistence, LAPS, and Okta identity management in partnership with cybersecurity leadership.

Built operational processes aligned to CMMC 2.0 control requirements and produced audit-ready evidence habits.

Co-designed an always-on Palo Alto GlobalProtect VPN approach so new devices could join domain, receive GPOs, and access internal resources securely from first boot.

Outcome:

Stronger privileged access controls and improved identity/endpoint alignment.

Increased reliability of management posture for remote/distributed devices.

Tools: Okta, LAPS, Absolute Persistence, Palo Alto GlobalProtect, AD/GPO, compliance reporting/audit trails

3) Platform Modernization: Intune Stand-Up + Apple Ecosystem + Packaging Automation

Problem: Reduce drift, manual work, and inconsistent device posture by standing up a real endpoint management baseline and automating packaging/update workflows.

Scope: Large Windows fleet plus mobile; Apple ecosystem integration; packaging automation and UEM data quality.

Approach (Intune/Apple):

Took an Intune tenant that existed “on paper” and stood up core capabilities end-to-end.

Integrated Apple Business Manager (ABM) + VPP and built baseline compliance/configuration policies.

Standardized enrollment patterns and produced runbooks to make operations repeatable.

Approach (Packaging/Automation):

Built a modular PowerShell packaging framework with structured logging.

Created Python automation for version detection/validation (web parsing + regex).

Implemented JSON-driven REST API integration to populate UEM metadata (vendor/version/dependencies).

Established Git/Bitbucket workflows (branch-per-engineer + merge discipline) to scale collaboration.

Outcome:

More consistent device posture and reduced operational drift.

Reduced manual packaging/metadata work; improved repeatability and traceability.

Tools: Intune, ABM/VPP, PowerShell, Python, REST APIs/JSON, Git/Bitbucket, Workspace ONE UEM, ServiceNow KB/runbooks

Decision Record (POC/Evaluation): Jamf Pro vs Intune for macOS/mobile

Context: Evaluated Jamf Pro as part of endpoint platform architecture planning.
Result: Selected Intune for mobile devices and macOS management based on operational fit, identity/security alignment, and tooling consolidation goals.
(Note: evaluation/POC work; not claiming Jamf Pro administration at Jamf 300+ level.)

What I can share in interviews

Change control approach (testing, comms, rollback)

Platform design decisions and tradeoffs

Example runbook structure and documentation patterns

High-level automation patterns (without proprietary code)
