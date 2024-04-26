---
title: "Information Security Policy Framework"
author: "2242090"
bibliography: references.bib
csl: harvard-imperial-college-london.csl
geometry: "left=1.75cm, right=1.75cm, top=1.75cm, bottom=1.75cm, landscape"
---

---

# 1 Policies

| Policy                      | Purpose                                                                                                              |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Data protection             | Ensuring the confidentiality, integrity, and availability of sensitive data                                          |
| Access control              | Defining rules regarding granting, revoking, and managing access to data based on business and security requirements |
| Risk management             | Outlining processes for identifying, mitigating, and assessing security risks across the IT infrastructure           |
| Encryption                  | Description of the cryptographic protocols used to protect sensitive data at rest, in transit, and when backing up   |
| Secure configuration        | Baselines for server hardening, network, and endpoint devices to be secure against vulnerabilities                   |
| Change management           | The mechanism for integrating any new changes (such as new devices, protocols, etc.) into the IT infrastructure      |
| Incident response           | Methods for detecting, reporting, containing, and recovering from threat incidents                                   |
| Backup & recovery           | Operations for backing up data, how data is securely stored, and recovery protocols from data disruptions            |
| Acceptable use              | Regulations for appropriate use of components of the IT infrastructure for employees                                 |
| Vulnerability management    | Mechanisms for identifying, categorising, evaluating, and mitigating in systems in the IT infrastructure             |
| Network security            | Guidelines for technical network controls, such as firewalls, remote access protocols, etc.                          |
| Email/web security          | Methods for email filtering, anti-spam, anti-malware, web filtering, etc.                                            |
| Physical security           | Controls for physical access, regarding equipment security and environmental access                                  |
| Personnel security          | Employee security, such as background checks, security awareness, training, etc.                                     |
| Secure development practice | Secure coding practices, suitable testing frameworks, and SDLC (Software Development Life Cycle)                     |

# 2 Mapping policies to relevant standards

| Policy                      | Relevant standard                                                                                                    |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Data protection             | UK Data Protection Act 2018 [@govuk2018], GDPR [@eu2016]                                                             |
| Access control              | NIST 800-171 (3.1) Access Control [@nist2020], UK Government Security Policy Framework [@govuk2022]                  |
| Risk management             | NIST SP 800-39 [@nist2011], ISO 27001 [@iso2022], UK Cyber Essentials [@ncsc2023]                                    |
| Encryption                  | FIPS 140-2 [@nist2001], NCSC Encryption Guidelines [@ncsc2022]                                                       |
| Secure configuration        | NCSC End User Device Security Guidance [@2ncsc2022], CIS Benchmarks (multiple benchmarks, operating system specific) |
| Change management           | ITIL Change Management [@freshservice], UK Government Technology Code of Practice [@govuk2021]                       |
| Incident response           | NIST 800-61 [@nist2012], UK GDPR Article 33 [@intersoftconsulting]                                                   |
| Backup & recovery           | UK Government Cloud Security Principles [@govuk2014]                                                                 |
| Acceptable use              | UK Government Security Policy Framework [@govuk2022]                                                                 |
| Vulnerability management    | NCSC Vulnerability Management Guidance [@ncsc2024]                                                                   |
| Network security            | UK NCSC Network Security Guidance [@2ncsc2022]                                                                       |
| Email/web security          | NCSC Guidance on Email/Web Security [@ncsc2019]                                                                      |
| Physical security           | UK Government Security Requirements [@2govuk2021]                                                                    |
| Personnel security          | UK Government Personnel Security Controls [@ukgov2018]                                                               |
| Secure development practice | OWASP Secure Coding Practices [@owasp2010]                                                                           |

# 3 Policy priority

The $Priority$ column is categorised as:

- $High$: critical policies core to the IT infrastructure
- $Medium$: Important supporting policies, but less critical

| Policy                      | Priority |
| --------------------------- | -------- |
| Data protection             | High     |
| Access control              | High     |
| Risk management             | High     |
| Encryption                  | High     |
| Secure configuration        | High     |
| Change management           | Medium   |
| Incident response           | High     |
| Backup & recovery           | High     |
| Acceptable use              | Medium   |
| Vulnerability management    | High     |
| Network security            | High     |
| Email/web security          | Medium   |
| Physical security           | Medium   |
| Personnel security          | Medium   |
| Secure development practice | Medium   |

# 4 Mapping policies to applicable components of the IT infrastructure

| Policy                      | Applicable components                                                                               |
| --------------------------- | --------------------------------------------------------------------------------------------------- |
| Data protection             | - Active Directory <br> - ERP systems <br> - Email/file servers <br> - All endpoints (PCs/Laptops)  |
| Access control              | - Systems handling sensitive data <br> - Backup infrastructure <br> - Data flows with third-parties |
| Risk management             | - All IT systems, applications, data assets <br> - Business processes                               |
| Encryption                  | - Servers <br> - Endpoints <br> - Backups <br> - Data transfers                                     |
| Secure configuration        | - Windows servers <br> - Linux Web servers <br> - Network devices <br> - Endpoints                  |
| Change management           | - All IT systems and infrastructure changes                                                         |
| Incident response           | - All IT components <br> - Physical security                                                        |
| Backup & recovery           | - Servers <br> - Critical applications <br> - Backup systems                                        |
| Acceptable use              | - All endpoints (PCs/Laptops) <br> - Remote access                                                  |
| Vulnerability management    | - All IT assets <br> - Web applications                                                             |
| Network security            | - Firewalls <br> - Network zones <br> - Remote access                                               |
| Email/web security          | - Email servers <br> - Web servers <br> - Endpoints                                                 |
| Physical security           | - Facilities <br> - Data centers <br> - Equipment                                                   |
| Personnel security          | - HR processes <br> - Employee lifecycle                                                            |
| Secure development practice | - R&D engineering environment                                                                       |
