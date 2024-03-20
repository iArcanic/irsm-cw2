---
title: "Information Security Policy Framework"
author: "Preetham Ananthkumar – 2242090"
bibliography: references.bib
csl: harvard-imperial-college-london.csl
geometry: "left=1.25cm, right=1.25cm, top=1.25cm, bottom=1.25cm, landscape"
---

---

The $Priority$ column is categorised as:

- $High$: critical policies that are core to the IT infrastructure and should be addressed first
- $Medium$: Important supporting policies, but much less critical in relation to those labelled as $High$

| Policy/procedure category   | Purpose                                                                                                                                | Relevant standards/control                                                                                           | Priority |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------- |
| Data protection             | The means of ensuring the confidentiality, integrity, and availability of sensitive data                                               | UK Data Protection Act 2018 [@govuk2018], GDPR [@eu2016]                                                             | High     |
| Access control              | Definition for rules regarding granting, revoking, and managing access to data based on business and security requirements             | NIST 800-171 (3.1) Access Control [@nist2020], UK Government Security Policy Framework [@govuk2022]                  | High     |
| Risk management             | Outline the processes for identifying, mitigating, and assessing security risks across the IT infrastructure                           | NIST SP 800-39 [@nist2011], ISO 27001 [@iso2022], UK Cyber Essentials [@ncsc2023]                                    | High     |
| Encryption                  | Description of the cryptographic protocols used to protect sensitive data at rest, in transit, and when backing up                     | FIPS 140-2 [@nist2001], NCSC Encryption Guidelines [@ncsc2022]                                                       | High     |
| Secure configuration        | Baselines concerning server hardening, network, and endpoint devices to be secure against the latest vulnerabilities                   | NCSC End User Device Security Guidance [@2ncsc2022], CIS Benchmarks (multiple benchmarks, operating system specific) | High     |
| Change management           | The mechanism for integrating any new changes (such as new devices, protocols, etc.) into the current IT infrastructure                | ITIL Change Management [@freshservice], UK Government Technology Code of Practice [@govuk2021]                       | Medium   |
| Incident response           | Methods for detecting, reporting, containing, and recovering from threat incidents and breaches of personal data                       | NIST 800-61 [@nist2012], UK GDPR Article 33 [@intersoftconsulting]                                                   | High     |
| Backup and recovery         | Operations for backing up data, how data is securely stored, and recovery protocols from data disruptions                              | UK Government Cloud Security Principles [@govuk2014]                                                                 | High     |
| Acceptable use              | Regulations with regard to appropriate use of components of the IT infrastructure (such as systems, devices, data, etc.) for employees | UK Government Security Policy Framework [@govuk2022]                                                                 | Medium   |
| Vulnerability management    | Mechanisms for identifying, categorising, evaluating, and mitigating in systems in the IT infrastructure                               | NCSC Vulnerability Management Guidance [@ncsc2024]                                                                   | High     |
| Network security            | Guidelines for technical network controls, such as firewalls, segmentation, remote access protocols, etc.                              | UK NCSC Network Security Guidance [@2ncsc2022]                                                                       | High     |
| Email/web security          | Methods for email filtering, anti-spam, anti-virus, anti-malware, web filtering, etc.                                                  | NCSC Guidance on Email/Web Security [@ncsc2019]                                                                      | Medium   |
| Physical security           | Means of controls for physical access, regarding equipment security and environmental access through measures such as biometrics       | UK Government Security Requirements [@2govuk2021]                                                                    | Medium   |
| Personnel security          | Regarding employee security, such as background checks, security awareness, training, etc.                                             | UK Government Personnel Security Controls [@ukgov2018]                                                               | Medium   |
| Secure development practice | Secure coding practices, suitable testing frameworks, and SDLC (Software Development Life Cycle)                                       | OWASP Secure Coding Practices [@owasp2010]                                                                           | Medium   |
