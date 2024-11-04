---
layout: col-sidebar
title: OWASP Cloud-Native Application Security Top 10
site_side: true
tags: cloud-native-application-security
level: 2
type: documentation
auto-migrated: 0
pitch: The primary goal of the OWASP Cloud-Native Application Security Top 10 document is to provide assistance and education for organizations looking to adopt Cloud-Native Applications securely. The guide provides information about what are the most prominent security risks for Cloud-Native applications, the challenges involved, and how to overcome them.
---
[![Follow on Twitter](https://img.shields.io/twitter/follow/owaspcloudnati1?label=Follow%20%40owaspcloudnati1&style=social)](https://twitter.com/owaspcloudnati1)
## Overview

**Important Note:** This project is **very much alive**, and was last updates in April 2022. We are currently looking for contributors willing to draft the different categories, so please feel free to drop us an email if you would like to assist.

Cloud native technologies empower organizations to build and run scalable applications in modern, dynamic environments such as public, private, and hybrid clouds. Containers, service meshes, microservices, immutable infrastructure, and declarative APIs exemplify this approach. Cloud-Native applications are a fundamentally new and exciting approach to designing and building software. However, it also raises a completely new set of security challenges. For example, when you move to a microservice model, end-to-end visibility, monitoring and detection become more complex and difficult to execute.
<br>
<br>
The primary goal of the OWASP Cloud-Native Application Security Top 10 document is to provide assistance and education for organizations looking to adopt Cloud-Native applications securely. The guide provides information about what are the most prominent security risks for cloud-native applications, the challenges involved, and how to overcome them.

## Interim List of Risks - Currently Under Review!

The OWASP Cloud-Native Top 10 list is currently under development (July 2021). As part of our effort to collect feedback, we are presenting an interim list below. Please feel free to contact the project leaders if you have any feedback. 

#### [CNAS-1: Insecure cloud, container or orchestration configuration][CNAS1:2022]
Examples:
 * Publicly open cloud storage buckets
 * Improper permissions set on cloud storage buckets
 * Container runs as root
 * Container shares resources with the host (network interface, etc.)
 * Insecure Infrastructure-as-Code (IaC) configuration
 * ...

#### [CNAS-2: Injection flaws (app layer, cloud events, cloud services)][CNAS2:2022]
Examples:
 * SQL injection
 * XXE
 * NoSQL injection
 * OS command injection
 * Serverless event data injection
 * ...

#### [CNAS-3: Improper authentication & authorization][CNAS3:2022]
Examples:
 * Unauthenticated API access on a microservice
 * Over-permissive cloud IAM role
 * Lack of orchestrator node trust rules (e.g. unauthorized hosts joining the cluster)
 * Unauthenticated orchestrator console access 
 * Unauthrized or overly-permissive orchestrator access

#### [CNAS-4: CI/CD pipeline & software supply chain flaws][CNAS4:2022]
Examples:
 * Insufficient authentication on CI/CD pipeline systems
 * Use of untrusted images 
 * Use of stale images
 * Insecure communication channels to registries
 * Overly-permissive registry access 
 * Using a single environment to run CI/CD tasks for projects requiring different levels of security
 * ...

#### [CNAS-5: Insecure secrets storage][CNAS5:2022]
Examples:
 * Orchestrator secrets stored unencrypted
 * API keys or passwords stored unencrypted inside containers
 * Hardcoded application secrets
 * Poorly encrypted secrets (e.g. use of obsolete encryption methods, use of encoding instead of encryption, etc.) 
 * Mounting of storage containing sensitive information
 * ...

#### [CNAS-6: Over-permissive or insecure network policies][CNAS6:2022]
Examples:
 * Over-permissive pod to pod communication allowed
 * Internal microservices exposed to the public Internet
 * No network segmentation defined
 * End-to-end communications not encrypted
 * Network traffic to unknown or potentially malicious domains not monitored and blocked
 * ...

#### [CNAS-7: Using components with known vulnerabilities][CNAS7:2022]
Examples:
 * Vulnerable 3rd party open source packages
 * Vulnerable versions of application components
 * Use of known vulnerable container images
 * ...

#### [CNAS-8: Improper assets management][CNAS8:2022]
Examples:
 * Undocumented microservices & APIs
 * Obsolete & unmanaged cloud resources
 * ...

#### [CNAS-9: Inadequate 'compute' resource quota limits][CNAS9:2022]
Examples:
 * Resource-unbound containers
 * Over-permissive request quota set on APIs
 * ...

#### [CNAS-10: Ineffective logging & monitoring (e.g. runtime activity)][CNAS10:2022]
Examples:
 * No container or host process activity monitoring
 * No network communications monitoring among microservices
 * No resource consumption monitoring to ensure availability of critical resources
 * Lack of monitoring on orchestration configuration propagation and stale configs
 * ...

## Getting Involved
You do not have to be a security expert or a programmer to contribute. Contact the project leader(s) to get involved, we welcome any type of suggestion and comments. Possible ways to contribute:
 * We are actively looking for organizations and individuals that will provide vulnerability prevalence data
 * Translation efforts (later stages)
 * Individuals and organizations that will contribute to the project will be listed on the acknowledgments page.

[CNAS1:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x01_insecure_cco_config.md  
[CNAS2:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x02_inj_flaws.md
[CNAS3:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x03_improper_auth.md
[CNAS4:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x04_cicd_ssc_flaws.md
[CNAS5:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x05_insecure_secrets.md
[CNAS6:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x06_over_permissive_network.md
[CNAS7:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x07_vuln_components.md
[CNAS8:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x08_asset_mgmt.md
[CNAS9:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x09_compute_resources.md
[CNAS10:2022]: https://github.com/OWASP/www-project-cloud-native-application-security-top-10/blob/master/2022/en/src/0x0A_logging.md
