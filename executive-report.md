---
title: "Executive Report"
author: "Preetham Ananthkumar – 2242090"
bibliography: references.bib
toc: true
toc-title: Table of Contents
toc-depth: 3
csl: harvard-imperial-college-london.csl
---

---

# 1 Introduction

<!-- 150-200 words -->

This executive report provides a brief but comprehensive insight into the proposed Information Security Policy Framework containing policies and procedures that are specifically designed for the company to be compliant with UK governmental security requirements. Since this is a "high-priority", "high-visibility" project with a significant revenue incentive (30%), it is important to demonstrate relevant compliance with all necessary regulations.

The mentioned framework covers a wide range of policy areas, most notably data protection, secure configurations, risk management, access controls, incident response, and much more. The policies are matched to an according UK standards, such as NCSC guidelines, the Data Protection Act 2018, and NIST controls, to name a few.

Integrating this framework into the company's IT infrastructure, will not only secure the company's assets (i.e. systems and data assets) but also guarantee that it satisfies contracts with the UK Government. The report will also address policies and procedures which are marked as "$High$" within the framework, as well as key security controls to deal with them, supporting policies marked as "$Medium$" which supplement the main policies, and finally a high-level implementation plan to practically meet the criteria of this framework.

The recommendations and the plan provided by the framework, if adopted correctly by the company, can demonstrate its competence in its information security practices, and risk mitigation as identified in the previous risk assessment, and form a robust security foundation for the company that will undoubtedly help with future contracts.

# 2 High priority policies and procedures

<!-- 600-700 words -->

## 2.1 Access Control Policy

<!-- 150-200 words -->

A strong Access Control Policy ensures that only authorised individuals of the organisation can access components of the IT infrastructure, data, systems, and applications based on their permissions and applicable business needs. By enforcing the principle of least privilege in line with Article 5 of GDPR [@intersoftconsulting2], it will limit access rights for users to perform their necessary job functions. By deliberating excess permissions can increase risks of insider threats and potentially result in internal data breaches.

This policy is in alignment with access control requirements detailed in the NIST Special Publication 800-171 [@nist2020] and the UK Government Security Policy Framework [@govuk2022]. Key elements of this policy will include:

- Regular reviews of user access rights with the intention to promote lesser privileges
- Multi-factor authentication algorithms for systems that handle sensitive data
- Stricter controls around admin-level access systems
- Logging and monitoring mechanisms
- Swiftly revoking access for terminated employees

This policy, enforced through technical controls too, is vital for managing which users have access company assets to prevent unathorised access.

## 2.2 Data Protection Policy

<!-- 150-200 words -->

Securing the confidentiality, integrity, and availability of the company's data is essential. Therefore, this Data Protection Policy will outline some measures that are compliant with both the UK Data Protection Act 2018 [@govuk2018] and UK GDPR [@eu2016] requirements.

Key aspects of this policy will include:

- Data classification guidelines to accurately define what data is sensitive
- Breach notifications and processes that are in compliance with GDPR Article 33 [@intersoftconsulting]
- Clear defines roles and responsibilities for both data owners and users
- Compulsory security awareness training for users and employees to undergo before interacting with company systems
- Third-party data processing management and controls
- Processes and procedures for data handling including its lifecycle (i.e. creation and destruction)
- Technical controls, such as encryption, logging, access restrictions, and so on

The rigorous enforcement of this policy will arguably help to protect one of the company's most important assets and demonstrate to governments a strong commitment to ensuring, at all times, the confidentiality, integrity, and availability of this data.

## 2.3 Risk Management Policy

A fully encompassing Risk Management Policy is intrinsic to forming a workable information security program. The policy will encourage systematic and regular risk assessments to be conducted (similar to the previous one) across the IT infrastructure landscape, including people, processes, systems, applications, data, and any other related assets. Potential risks will be identified as a result of this, and are rated by their likelihood of occurring and the impact that they would have on general business operations.

This Risk Management Policy was inspired by best practice frameworks such as NIST SP 800-39 [@nist2011] and ISO 27001 [@iso2022] whilst also in alignment with the UK Government's Cyber Essentials [@ncsc2023]. This policy takes into account the following criteria:

- Identifying vulnerable assets, threats they are at risk to, and risk scenarios
- Calculating the impact of risk exposure both quantitatively and qualitatively
- Selecting and deciding the best implementation techniques on risk treatment options
- Deciding upon a long term risk monitoring and review process

Integrating the specific security controls and measures will be heavily influenced by the risks identified in the risk register and recommendations as a result of the risk assessment. Such an approach can confirm that resources and security efforts are coordinated to be efficiently focussed on mitigating the highest priority risks to the company.

## 2.4 Encryption Policy

<!-- 150-200 words -->

Encryptions controls will allow for any sensitive data that the company holds to be effectively retained securely for its confidentiality but also to comply with UK governmental standards. This Encryption Policy will serve as a directive to use industry level cryptographic algorithms across the IT infrastructure landscape.

This policy considers data when its in three different states:

- Data at rest: all confidential data stored on endpoint devices, removable media, servers, backups, and so on must be encrypted using a protocol mentioned in NIST's FIPS 140-2 [@nist2001] with a key of a suitable length that balances both performance and security
- Data in transit: transmission of sensitive data taking place over untrusted or public networks should utilise technical protocols with authorised cipher suites
- Backup data: Confidential data should be encrypted effectively to protect against breaches or exposure risks during either transit or storage

Regarding cryptographic key management, this policy also specifies requirements with respect to key management lifecycle stages [@warner2022]. Those being periodic key rotation, recovery processes, key storage, and retrieval, all in alignment with NCSC guidelines [@ncsc2022].

In addition, this policy also disallows the use of third-party or insecure cryptographic algorithms that are not widely recognised or documented by standards such as NIST or FIPS or included within the the UK government cipher recommendations.

Regular attention to this Encryption Policy will allow for sensitive data to be protected at all times and enforce regulatory compliance.

## 2.5 Secure Configuration Policy

<!-- 150-200 words -->

A hardening criteria and secure configuration baseline is foundational for minimising the attack surface on the company's technology assets. The Secure Configuration Policy determines strict standards and settings needed for securing technical assets such as servers, network devices, and endpoint devices to stop threat actors from exploiting weak configurations.

Within the IT infrastructure, particularly for components such as servers and network devices, it is recommended to follow the vendor's hardening guidelines rather than individual configuration. This is in agreement with Centre of Internet Security (CIS) benchmarks, that are provided for each type of device and operating system. It means that areas like applying the latest patches, security logging, and unnecessary service disabling are all covered.

In the same way for endpoint devices such as employee workstations are laptops, the policy entails that the NCSC End User Device (EUD) Security Guidance [@2ncsc2022] along with the appropriate CIS benchmarks be consolidated within the IT infrastructure for a robust defense.

The policy will mandate formality when managing configurations, and also when migrating from one hardening baseline to another. Variations need to be approved to ensure that they follow verified benchmarks and have a risk assessment conducted upon it. The result from this assessment will provide confidence that the existing IT infrastructure is not compromised. Furthermore, it should also be throughly tested in a production environment and monitored for a short period of time before it can be fully marked as functional and secure.

# 3 Key security controls

<!-- 400-500 words -->

## 3.1 Access controls

<!-- 100 words -->

Access controls will be implemented via a unified Identity Access Management (IAM) system. Through this, it will include:

- A Role-Based Access Control (RBAC) scheme for controlling permissions on a granular level
- Automated and periodic user account activation and deactivation
- Audit logging and monitoring schemes of access activities and permission granting or revoking
- Multi-factor authentication protocols for access to high risk or admin systems

These IAM controls will span across the whole IT infrastructure landscape such as on-site system, cloud applications, and external third-party systems. It also fits in with the principle of least privilege.

## 3.2 Data protection controls

<!-- 100 words -->

Data protection controls will maintain the confidentiality, integrity, and availability of the company's sensitive data assets. These include:

- Data classification and post processing actions based on sensitivity and value of the data
- Data loss prevention mechanisms to help recover data in the event of unauthorised data usage or transfer
- Secure backup schemes with thorough data restoration protocols and offsite storage
- Encryption of data at rest, in transit, and when being backed-up

Having multi-layered controls makes it significantly harder when a malicious threat actor intents to penetrate security defences.

## 3.3 Risk management controls

<!-- 100 words -->

## 3.4 Cryptographic controls

<!-- 100 words -->

## 3.5 Secure baseline configurations

<!-- 100 words -->

# 4 Supporting policies

<!-- 300-400 words -->

# 5 Implementation approach

<!-- 400-500 words -->

# 6 Appendices

# 7 Bibliography
