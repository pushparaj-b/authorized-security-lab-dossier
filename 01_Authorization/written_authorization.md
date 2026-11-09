# Authorized Security Lab — Written Authorization Record

**Project:** Legal Scope, Asset Inventory & Threat Model  
**Assessment type:** Controlled security assessment and threat modeling  
**Prepared by:** Student / Security Analyst (enter your name)  
**Lab owner:** RabTech lab (as identified in the supplied starter inventory)  
**Prepared on:** 09 November 2026  
**Authorization status:** **PENDING — owner approval and approved testing window must be obtained before any testing.**

## 1. Purpose
This engagement plan defines the assets, boundaries, risks, evidence controls, and stop conditions for a controlled security assessment in an isolated training environment.

## 2. Approved-inventory targets
- **LAB-01:** Local training web app — `http://127.0.0.1:8080`
- **LAB-02:** Deliberately vulnerable VM — `192.168.56.20` on a private host-only network

The inventory is transcribed from the starter material supplied for this task. Inclusion in the inventory is not, by itself, proof that the assessor has received authorization to test.

## 3. Authorization conditions
Before testing begins, the lab owner or authorized representative must confirm in writing:
- the assessor's identity;
- that the listed assets are under the owner's control and available for this exercise;
- the exact testing start/end date and time;
- the permitted techniques and rate limits;
- an emergency contact and escalation route.

**Owner approval / signature:** ____________________  
**Approval date:** ____________________  
**Approved testing window:** ____________________  
**Emergency contact:** ____________________

## 4. Scope exclusions
No testing of public websites, third-party systems, personal devices, unlisted IP addresses, or systems discovered incidentally. No denial of service, destructive payloads, persistence, credential theft/reuse, malware deployment, uncontrolled data extraction, or outbound traffic from the isolated VM.

## 5. Proposed lab implementation note
If the supplied LAB-01 application is unavailable, OWASP Juice Shop may be proposed as a local training substitute only after the lab owner/instructor approves the substitution. Do not represent it as the supplied RabTech application. LAB-02 must not be marked implemented until the actual VM image is supplied, configured, and its address verified.

## 6. Current implementation status
This dossier is a planning and documentation package. It does not claim that Docker, Juice Shop, VirtualBox, or the supplied VM has been installed or tested. Complete the implementation evidence checklist after performing the steps on your own computer.
