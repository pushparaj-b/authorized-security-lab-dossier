# Authorized Security Lab — Rules of Engagement

**Project:** Legal Scope, Asset Inventory & Threat Model  
**Assessor:** Student / Security Analyst (enter your name)  
**Lab owner:** RabTech lab (approval pending)  
**Status:** Draft — no active testing until approved.

## 1. Authorization and scope
Only the assets explicitly listed in `authorized-lab-assets.csv` are in scope:
- LAB-01 — `http://127.0.0.1:8080`
- LAB-02 — `192.168.56.20` on a private host-only network

The owner must approve the assessor, assets, techniques, and testing window in writing. An asset appearing in the starter CSV does not independently establish permission.

## 2. Permitted activities (after approval)
- Review the lab architecture and configuration.
- Non-destructive asset and service identification limited to approved assets.
- Review authentication, authorization, input validation, and security headers using test accounts and synthetic data.
- Perform safe manual validation of documented threat scenarios.
- Capture minimal evidence and prepare remediation recommendations.

## 3. Explicit exclusions
- Denial-of-service or stress testing.
- Destructive or irreversible payloads.
- Persistence, malware, backdoors, or privilege retention.
- Credential theft, password spraying, or reuse of real credentials.
- Third-party scanning or testing unlisted assets.
- Uncontrolled data extraction or access to real personal data.
- Outbound traffic from the host-only VM.
- Social engineering or phishing.

## 4. Testing window and operating limits
**Start:** To be approved by lab owner.  
**End:** To be approved by lab owner.  
**Time zone:** India Standard Time (IST), unless the owner specifies otherwise.  
**Rate limits:** Use conservative, owner-approved request rates; stop if instability is observed.  
**Emergency contact:** To be supplied by lab owner.  
No testing outside the approved window.

## 5. Stop conditions
Stop immediately and notify the owner if:
- a target does not match the approved inventory;
- an unexpected outage, instability, or performance degradation occurs;
- traffic leaves the isolated lab or an external system is contacted;
- real personal data, secrets, or credentials are exposed;
- an action risks data loss or service disruption;
- the owner withdraws authorization or requests a stop.

Do not attempt to investigate beyond the approved boundary after a stop condition.

## 6. Evidence handling
- Use synthetic test data and dedicated test accounts only.
- Collect the minimum evidence needed to support a finding.
- Redact passwords, tokens, session identifiers, personal data, and unrelated information.
- Store evidence in the restricted project folder.
- Do not publish sensitive evidence in a public repository.
- Agree the retention and deletion date with the owner before testing.

## 7. Reporting
Each finding must include: finding ID, affected asset, description, evidence reference, severity rationale, impact, safe reproduction steps, recommended remediation, and validation status. Distinguish confirmed observations from hypotheses.

## 8. Approval record
**Owner/authorized representative:** ____________________  
**Signature or written approval reference:** ____________________  
**Date:** ____________________  
**Assessor acknowledgment:** ____________________  
**Date:** ____________________
