---
title: "Executive Report"
author: "Preetham Ananthkumar – 2242090"
bibliography: references.bib
geometry: "left=1.25cm, right=1.25cm, top=1.25cm, bottom=1.25cm"
csl: harvard-imperial-college-london.csl
---

# 1 Introduction

This executive report provides a brief but comprehensive insight into the Information Security Policy Framework containing policies that are specifically designed for the high-tech 400 employee company to be compliant with UK governmental security requirements. Since this is a "high-priority", "high-visibility" project with a revenue incentive of 30%, it is important to demonstrate compliance with all necessary regulations. It's worth nothing that currently, the company doesn't have any controls that are government compliant.

The framework covers a wide range of policy areas. The policies are matched to an according UK standards, such as NCSC guidelines, the Data Protection Act 2018 [@govuk2018], and NIST controls.

Integrating this framework into the IT infrastructure, will not only secure the company's assets but also guarantee that it satisfies contracts with the UK Government. The report will address policies which are marked as "$High$" within the framework, as well as key security controls to deal with them, and a high-level implementation plan to practically meet the criteria of this framework.

The recommendations provided by the framework, if adopted correctly by the company, can demonstrate competence in information security practices, risk mitigation, and form a security foundation for the company that will help with future contracts.

# 2 High priority policies and procedures

## 2.1 Access Control Policy

An Access Control Policy ensures that only authorised individuals of the organisation can access components of the IT infrastructure, data, and systems based on their permissions and business needs. By enforcing the principle of least privilege in line with Article 5 of GDPR [@intersoftconsulting2], it will limit access rights for users to perform their necessary functions. Deliberating excess permissions can increase risks of insider threats and potentially result in data breaches. Specifically, this applies to the Active Directory environment, ERP applications, email servers, and all endpoint devices.

This policy is in alignment with access control requirements detailed in the NIST Special Publication 800-171 [@nist2020] and the UK Government Security Policy Framework [@govuk2022]. Key elements of this policy will include:

- Regular reviews of access rights with the intention to promote lesser privileges
- Multi-factor authentication algorithms for systems handling sensitive data
- Stricter controls around admin-level access systems
- Logging and monitoring mechanisms
- Swiftly revoking access for terminated employees

This policy is vital for managing which users have access company assets to prevent unathorised access.

## 2.2 Data Protection Policy

Securing the confidentiality, integrity, and availability of the company's data is essential. Therefore, this Data Protection Policy will outline some measures that are compliant with the UK Data Protection Act 2018 [@govuk2018] and UK GDPR [@eu2016] requirements.

Key aspects of this policy will include:

- Encrypting sensitive data in systems such as in ERP, email security solutions like Symantec, and other private stores
- Data classification guidelines to accurately define what data is sensitive
- Breach notifications and processes that are in compliance with GDPR Article 33 [@intersoftconsulting]
- Clear defines roles and responsibilities for both data owners and users
- Compulsory security awareness training for users and employees to undergo before interacting with company systems
- Third-party data processing management and controls
- Processes and procedures for data handling including its lifecycle (i.e. creation and destruction)
- Technical controls, such as encryption, logging, access restrictions, and so on

The enforcement of this policy will help to protect one of the company's most important assets and demonstrate to governments a strong commitment to ensuring the confidentiality, integrity, and availability of this data.

## 2.3 Risk Management Policy

A fully encompassing Risk Management Policy is intrinsic to forming a workable information security program. The policy will encourage regular risk assessments to be conducted across the IT infrastructure landscape (Windows Server, Active Directory, ERP, R&D, Linux systems), including people, processes, and data. Potential risks will be identified as a result of this, and are rated by their likelihood of occurring and their impact on business operations.

This Risk Management Policy was inspired by best practice frameworks such as NIST SP 800-39 [@nist2011] and ISO 27001 [@iso2022] whilst also in alignment with the UK Government's Cyber Essentials [@ncsc2023]. This policy takes into account the following criteria:

- Identifying vulnerable assets, threats they are at risk to, and risk scenarios
- Calculating the impact of risk exposure both quantitatively and qualitatively
- Selecting and deciding the best implementation techniques on risk treatment options
- Deciding upon a long term risk monitoring and review process

Integrating the specific security controls and measures will be heavily influenced by the risks identified in the risk register and recommendations from the risk assessment. Such an approach can confirm that resources and security efforts are coordinated to be efficiently focussed on mitigating the highest priority risks.

## 2.4 Encryption Policy

Encryptions controls will allow for any sensitive data that the company holds to be effectively retained securely for its confidentiality. This Encryption Policy will serve as a directive to use industry level cryptographic algorithms across the IT infrastructure.

This policy considers data when its in three different states:

- Data at rest: all confidential data stored on endpoint devices must be encrypted using a protocol mentioned in NIST's FIPS 140-2 [@nist2001] with a key of a suitable length that balances both performance and security
- Data in transit: transmission of sensitive data taking place over untrusted networks should utilise technical protocols
- Backup data: Confidential data should be encrypted effectively to protect against breaches or exposure risks during either transit or storage

Regarding cryptographic key management, this policy also specifies requirements with respect to key management lifecycle stages [@warner2022]. Those being periodic key rotation, recovery processes, key storage, and retrieval, all in alignment with NCSC guidelines [@ncsc2022].

In addition, this policy also disallows the use of third-party or insecure cryptographic algorithms that are not documented by standards such as NIST or FIPS or included within the the UK government cipher recommendations.

Regular attention to this Encryption Policy will allow for sensitive data to be protected at all times and enforce regulatory compliance.

## 2.5 Secure Configuration Policy

A secure configuration baseline is foundational for minimising the attack surface on the company's technology assets. The Secure Configuration Policy determines strict standards and settings needed for securing technical assets such as servers, network devices, and endpoint devices to stop threat actors from exploiting weak configurations.

It is recommended to follow the vendor's hardening guidelines rather than individual configuration. This is in agreement with Center of Internet Security (CIS) benchmarks, that are provided for each type of device and operating system, especially for server components such as Linux Ubuntu web servers and Windows Server 2022. It means that areas like applying the latest patches, security logging, and unnecessary service disabling are all covered.

The policy will mandate formality when managing configurations, and also when migrating from one hardening baseline to another. Variations need to be approved to ensure that they follow verified benchmarks and have risk assessments conducted. The result from this assessment will provide confidence that the existing IT infrastructure is not compromised.

# 3 Key security controls

## 3.1 Access controls

Access controls will be implemented via a unified Identity Access Management (IAM) system. Through this, it will include:

- A Role-Based Access Control (RBAC) scheme for controlling permissions on a granular level through integration with Active Directory
- Automated and periodic user account activation and deactivation via Microsoft Endpoint Manager
- Audit logging and monitoring schemes of access activities and permission granting or revoking such as Microsoft Event Viewer
- Multi-factor authentication protocols for access to Microsoft environments such as Active Directory and Exchange

These IAM controls will span across the whole IT infrastructure landscape such as on-site system, cloud applications, and external third-party systems. It also fits in with the principle of least privilege.

## 3.2 Data protection controls

Data protection controls will maintain the confidentiality, integrity, and availability of the company's sensitive data assets. These include:

- Data classification and post processing actions based on sensitivity and value of the data such as by using Microsoft BitLocker
- Data loss prevention mechanisms such as Microsoft Defender to help recover data in the event of unauthorised data usage or transfer
- Anti-malware scanning and email filtering through Symantec Email Security
- Secure backup schemes with thorough data restoration protocols and offsite storage
- Encryption of data at rest, in transit, and when being backed-up

Having multi-layered controls makes it significantly harder when a malicious threat actor intents to penetrate security defenses.

## 3.3 Risk management controls

In-depth risk management controls will help to methodically pinpoint, evaluate, and analyse information security risks across the company's IT infrastructure. For this, it will include:

- Continuous risk monitoring, suggested action paths, and reviews based on previous actions taken to address the risk
- Integration and synchronisation with other control areas, such as incident response and vulnerability management
- Thorough risk calculation method with factors such as impact, likelihood, and other factors
- Maintaining a company wide risk register that is constantly updated with the latest risks, threat scenarios, and vulnerability data from risk assessments conducted or credible cybersecurity vendors covering risks on Active Directory, Symantec products, and Microsoft Server

The controls here will lead to a more structured approach, where data is placed at the forefront. These controls are in agreement with well known frameworks such as NIST 800-39 [@nist2011] and ISO 27001 [@iso2022].

## 3.4 Cryptographic controls

Most of the along with the previous controls rely upon strong technical cryptographic measures to protect sensitive data. The controls should be appropriate for Microsoft environments. The ways in which this can be achieved are as follows:

- Only cryptographic modules, which are validated by FIPS 140-2 [@nist2001] with keys using of a minimum length of 256 bits
- AES encryption to be used for encryption of data at rest, or any other similar algorithm
- Data in transit over networks that are untrusted will use protocols such as TLS (exceeding version 1.2), SSH, and IPsec
- All stages in the cryptographic key management lifecycle should be thoroughly documented and updated if any changed do occur
- Verify key storage means, such as if the Public Key Infrastructure (PKI) and Hardware Security Module (HSM) used are secure themselves
- Any insecure algorithms, protocols, ciphers, or cryptography logic that does not confirm to the NIST's FIPS 140-2 [@nist2001] framework or NCSC guidelines will be disallowed

The controls here, based on certified cybersecurity frameworks and industry best practices will help in providing strong protection against threats concerning data.

## 3.5 Secure baseline configurations

Secure baseline configurations with hardening guidelines can considerably reduce the attack surface from threats on company systems and endpoint devices. This can be through:

- Implementation of Center for Internet Security (CIS) benchmark recommendations based on the specific OS being used for servers, network devices, and so on
- Removal and disabling of unused services, protocols, and ports based on results of a technical risk assessment
- Consistent and regular patches from credible and official sources only, such as Microsoft
- Following the Change Management Policy when business needs require deviations from established baselines
- Reliable security logging, auditing, monitoring, and informative documentation on activities of IT components
- Using built-in Microsoft security configurations and server templates

Aligning secure baseline configurations with industry standard recommendations will help in remediating vulnerabilities.

# 4 Implementation approach

A practical implementation of the framework will require a deployment plan, change management processes, and defined responsibilities spanning the organisation. With this, the company can effectively adhere to the Information Security Framework sustainably.

## 4.1 Deployment plan

The implementation of this framework will followed an approach separated into phases. Each phase will prioritise a vital security aspect to help get all IT components to the required compliance level.

### 4.1.1 Phase 1: Demonstrate oversight and governance

- Form a reliable information security governance committee with sponsorship from company executives
- Have clear security roles allocated to qualified individuals, those being CISO, administrators (both technical and non-technical), and security designers
- From the Risk Management Policy, enforce a risk management program
- Carry out a gap analysis on the existing IT infrastructure against the defined policies to establish a compliance baseline

### 4.1.2 Phase 2: Consider baseline controls

- From the Secure Configuration Policy, administer secure configuration for IT infrastructure components (endpoint devices, servers, networks)
- Access controls, permission, and identity management should be implemented
- Incident response capabilities should be set up, including security monitoring and logging

### 4.1.3 Phase 3: Prioritise data protection

- Enforce regulatory compliance, such as with the Data Protection Act 2018 [@govuk2018], GDPR [@eu2016], and so on
- Activate data protection controls, such as classification, Data Loss Prevention (DLP) tools, and encryption measures
- Establish data backup and recovery processes

## 4.2 Change management

Updates to the information security framework depending upon business needs need to follow all procedures outlined in the Change Management Policy. This involves:

- Conducted risk assessments, workflows tested and approved before integrating with the IT infrastructure
- Logging and auditing the implemented changes and their impacts, monitoring whether they compromise existing assets
- Have emergency provisions to rollback changes in the event that they jeopardise existing IT components

### 4.2.1 Roles and responsibilities

Having clear roles and responsibilities across multiple stakeholder categories, such as IT operations, management, and security teams will also be considered under change management processes.

- Executive sponsors: consists of a funding and resource program to support information security endeavors
- CISO/security teams: provide oversight into the program, help to maintain and implement policies, and oversee security operations
- IT operations: encompasses system administration, technical implementation of high-level controls
- Data owners: management of data usage, flows, and transfers
- Employees/company personnel: comply with the Acceptable Use Policy and undertake mandatory compliance training
- Third parties: confirm third party vendors that the company relies upon comply to a coordinated policy

# 5 Bibliography
